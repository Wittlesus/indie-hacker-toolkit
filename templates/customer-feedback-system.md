# Customer Feedback System

> A single source of truth for all customer feedback. Collect, organize, prioritize, and act on what your users are telling you.

---

## How This System Works (Read This First)

This isn't just a feedback tracker. It's a decision-making framework based on:

- **RICE Scoring** (Reach, Impact, Confidence, Effort) - Intercom's product prioritization model
- **Kano Model** - Classify features by customer satisfaction impact
- **Jobs-to-be-Done** - Understand the "why" behind feature requests

You'll find worked examples, interview scripts, and prioritization formulas below.

**Common Mistake:** Building features based on "number of requests" alone. 10 users requesting a feature doesn't mean it's important - they might all be edge cases. Use RICE scoring to make data-driven decisions.

---

## Feature Requests

Track every feature request in one place. Use the RICE scoring system to prioritize what to build next.

### RICE Scoring Guide (Use This, Not the Old Method)

**RICE = (Reach x Impact x Confidence) / Effort**

- **Reach:** How many users will this impact per month? (Actual number: 10, 50, 200, 1000, etc.)
- **Impact:** How much will this improve their experience? (3 = Massive, 2 = High, 1 = Medium, 0.5 = Low, 0.25 = Minimal)
- **Confidence:** How sure are you about Reach and Impact estimates? (100% = 1.0, 80% = 0.8, 50% = 0.5)
- **Effort:** Person-months to ship this. (0.5 = 2 weeks, 1 = 1 month, 2 = 2 months, etc.)

**RICE Score = (Reach x Impact x Confidence) / Effort** (Higher score = build first)

### Worked Example: Prioritizing 3 Feature Requests

| Feature | Reach | Impact | Confidence | Effort | RICE Score | Priority |
|---|---|---|---|---|---|---|
| **Dark mode** | 200 users/mo | 0.5 (Low - aesthetic) | 0.8 (80% sure) | 0.5 (2 weeks) | 160 | 2nd |
| **CSV export** | 50 users/mo | 2 (High - unblocks workflow) | 1.0 (100% sure) | 1 (1 month) | 100 | 3rd |
| **Slack integration** | 500 users/mo | 3 (Massive - daily use) | 0.5 (50% sure people will use it) | 2 (2 months) | 375 | **1st** |

**Decision:** Build Slack integration first, even though it's the most effort. It has the highest RICE score.

**Formula in action:**
- Dark mode: (200 x 0.5 x 0.8) / 0.5 = 160
- CSV export: (50 x 2 x 1.0) / 1 = 100
- Slack integration: (500 x 3 x 0.5) / 2 = 375

| # | Feature Request | Requested By | Reach | Impact | Confidence | Effort | RICE Score | Status | Target | Notes |
|---|---|---|---|---|---|---|---|---|---|---|
| 1 | Dark mode | @user1, @user2 | 200 | 0.5 | 0.8 | 0.5 | 160 | Planned | Q1 | 200 active users would use this |
| 2 | CSV export | @user3 | 50 | 2 | 1.0 | 1 | 100 | Backlog | -- | Only power users need this |
| 3 | Slack integration | @user4, @user5, @user6 | 500 | 3 | 0.5 | 2 | 375 | In Progress | Q1 | High reach, high impact, uncertain adoption |
| 4 | Mobile app | @user7 | 1000 | 2 | 0.3 | 6 | 100 | Won't Do | -- | Huge effort, low confidence it's needed |
| 5 | | | | | | | | | | |
| 6 | | | | | | | | | | |
| 7 | | | | | | | | | | |
| 8 | | | | | | | | | | |
| 9 | | | | | | | | | | |
| 10 | | | | | | | | | | |

**How to estimate Reach:** Look at your analytics. How many active users would realistically use this feature per month? Be conservative.

**How to estimate Impact:** Ask yourself: "If we ship this, how much does it improve the user's experience?"
- 3 (Massive): This becomes a core part of their daily workflow
- 2 (High): This unblocks them or saves significant time
- 1 (Medium): This makes their experience noticeably better
- 0.5 (Low): This is nice to have but not essential
- 0.25 (Minimal): This is purely cosmetic or edge-case

**How to estimate Confidence:** How certain are you about your Reach and Impact guesses?
- 1.0 (100%): You have data (surveys, user interviews, analytics)
- 0.8 (80%): You have qualitative feedback from multiple users
- 0.5 (50%): You have 1-2 requests, no strong evidence
- 0.2 (20%): Pure speculation

**How to estimate Effort:** In person-months. Be honest about scope creep.
- 0.25 = 1 week
- 0.5 = 2 weeks
- 1 = 1 month
- 2 = 2 months
- 4+ = Multi-month project (probably too big, break it down)

### Status Key
- **New** -- Just received, not yet reviewed
- **Under Review** -- Being evaluated for feasibility and priority
- **Planned** -- Accepted, scheduled for development
- **In Progress** -- Currently being built
- **Shipped** -- Live in production
- **Won't Do** -- Declined (always explain why to the requester)

---

## Bug Reports

Track and resolve bugs systematically. Prioritize by severity.

| # | Bug Description | Reported By | Date Reported | Severity | Steps to Reproduce | Status | Resolved Date | Notes |
|---|---|---|---|---|---|---|---|---|
| 1 | Example: Login fails on Safari mobile | @user1 | 2025-01-15 | Critical | 1. Open Safari on iPhone 2. Go to login page 3. Enter credentials 4. Tap "Log In" -- spinner never stops | Fixed | 2025-01-16 | WebKit auth cookie issue |
| 2 | Example: Dashboard chart shows wrong date range | @user2 | 2025-01-18 | Medium | 1. Go to Dashboard 2. Select "Last 30 days" 3. Chart shows 60-day range | In Progress | -- | Timezone offset bug |
| 3 | Example: Typo on pricing page | @user3 | 2025-01-20 | Low | 1. Visit /pricing 2. Second paragraph, "recieve" | Fixed | 2025-01-20 | Quick fix |
| 4 | | | | | | | | |
| 5 | | | | | | | | |
| 6 | | | | | | | | |
| 7 | | | | | | | | |
| 8 | | | | | | | | |

### Severity Levels
- **Critical** -- Product is broken for users. Data loss risk. Fix immediately.
- **High** -- Major feature is broken or unusable. Fix within 24-48 hours.
- **Medium** -- Feature works but with issues. Fix within 1 week.
- **Low** -- Minor cosmetic or UX issue. Fix when convenient.

---

## User Interviews Log

Talking to users is the highest-signal feedback channel. Log every conversation.

### The Kano Model: Categorize Features by Satisfaction Impact

Not all features are equal. The Kano Model helps you classify them:

**1. Must-Haves (Basic Needs):**
Features users expect. Absence causes dissatisfaction, but presence doesn't create delight.
- Example: User login, data security, core functionality working reliably
- **What to do:** Ship these first. They're table stakes.

**2. Performance Features (Satisfiers):**
Linear satisfaction. More = better. Users explicitly request these.
- Example: Faster load times, more integrations, better UI
- **What to do:** Improve these incrementally. They drive satisfaction.

**3. Delighters (Exciters):**
Unexpected features. Absence doesn't hurt, but presence creates delight and word-of-mouth.
- Example: Surprise free upgrade, handwritten thank-you note, hidden easter egg
- **What to do:** Sprinkle these in. They create emotional attachment.

**4. Indifferent:**
Users don't care either way.
- Example: Features you think are cool but nobody uses
- **What to do:** Don't build these. Cut scope ruthlessly.

**5. Reverse:**
Features that annoy some users.
- Example: Auto-play videos, aggressive upsell prompts, too many notifications
- **What to do:** Remove these if you detect them.

### How to Use Kano with Your Feature Requests

Ask users two questions for each feature:

1. "How would you feel if we **added** [feature]?" (5-point scale: I'd love it / I'd like it / I'm neutral / I'd dislike it / I'd hate it)
2. "How would you feel if we **didn't add** [feature]?" (Same scale)

Map responses:
- Love it if added + Neutral if not added = **Delighter**
- Love it if added + Hate it if not added = **Performance Feature**
- Neutral if added + Hate it if not added = **Must-Have**
- Neutral both ways = **Indifferent** (Don't build)

---

## User Interviews: The Complete Script

### Before the Call: Prep Checklist

- [ ] Review the user's account (When did they sign up? What features do they use? Any support tickets?)
- [ ] Prepare 8-10 questions (use template below)
- [ ] Set up recording (Zoom auto-record, get permission at start of call)
- [ ] Have a note-taking doc ready (or use Otter.ai for transcription)
- [ ] Block 45 minutes (30 min interview + 15 min buffer)

### Interview Script (Copy This)

**Opening (2 min):**
"Hey [name]! Thanks for taking the time. This should take about 30 minutes. I'm trying to understand how you use [product] and where we can improve. There are no wrong answers - honest feedback helps us build a better product. Do you mind if I record this so I don't miss anything?"

**Part 1: The Job-to-be-Done (10 min)**

These questions uncover the real problem the user is trying to solve.

1. "What made you sign up for [product] in the first place? Walk me through what was happening that day."
   - **Listen for:** The trigger event. What broke? What changed?

2. "What were you hoping [product] would help you accomplish?"
   - **Listen for:** The desired outcome, not the feature they wanted.

3. "Before [product], how were you solving this problem?"
   - **Listen for:** Workarounds, competitor tools, spreadsheets, manual processes.

4. "What made you switch from [old solution] to trying [product]?"
   - **Listen for:** Pain points with alternatives, urgency, budget triggers.

**Part 2: Current Experience (10 min)**

5. "Walk me through the last time you used [product]. What were you trying to do?"
   - **Listen for:** Their actual workflow, not what you think they do.

6. "What's the most valuable thing [product] does for you? If you could only keep one feature, what would it be?"
   - **Listen for:** Core value. Everything else is secondary.

7. "What's the most frustrating thing about [product] right now?"
   - **Listen for:** Friction points, missing features, confusing UX.

8. "Is there anything you've tried to do in [product] that you couldn't figure out?"
   - **Listen for:** Onboarding gaps, hidden features, unclear UI.

**Part 3: Future & Recommendation (5 min)**

9. "If you could wave a magic wand and change one thing about [product], what would it be?"
   - **Listen for:** Their #1 pain point in their own words.

10. "How would you feel if you could no longer use [product]? What would you do instead?"
   - **Listen for:** Switching cost, product stickiness. If they say "I'd be fine," you have a retention problem.

11. "Would you recommend [product] to a colleague or friend? Why or why not?"
   - **Listen for:** NPS signal. If yes, ask "who specifically?" and follow up with a referral request.

**Closing (3 min):**
"This was super helpful. A few quick logistics:
- Can I follow up if we build [thing they requested] to get your feedback?
- Would you be open to giving a testimonial if [product] has helped you?
- Any questions for me?"

Thank them. Send a $25 Amazon gift card or account credit within 24 hours.

### After the Call: Synthesis (15 min)

- [ ] Write down 3-5 key quotes (exact words)
- [ ] Identify: What job are they hiring the product to do?
- [ ] Note feature requests (add to Feature Requests table with RICE estimates)
- [ ] Note pain points (add to Bug Reports if actionable)
- [ ] Tag sentiment: Promoter (9-10), Passive (7-8), Detractor (0-6)
- [ ] Send thank-you email + gift card

### Interview Log

| # | User | Date | User Type | Key Quotes | Pain Points | Feature Requests | Follow-Up Actions |
|---|---|---|---|---|---|---|---|
| 1 | @user1 (Startup founder) | 2025-01-10 | Power user, Pro plan | "I love how fast it is." "I wish I could share reports with my team." | No team sharing, export is clunky | Team sharing, PDF export | Add team sharing to roadmap. Follow up in 2 weeks. |
| 2 | @user2 (Freelancer) | 2025-01-14 | Free trial, churned | "I couldn't figure out how to set up my first project." | Onboarding is confusing, no tutorial | Onboarding wizard, video walkthrough | Improve onboarding flow. Send re-engagement email. |
| 3 | @user3 (Agency) | 2025-01-20 | Enterprise prospect | "We need SSO and audit logs before we can buy." | Missing enterprise features | SSO, audit logs, role-based access | Scope enterprise tier. Follow up with pricing. |
| 4 | | | | | | | |
| 5 | | | | | | | |
| 6 | | | | | | | |

### Interview Insights Summary

After every 5 interviews, summarize patterns here:

**Batch 1 (Interviews 1-5):**
- Common pain point:
- Most requested feature:
- Biggest surprise:
- Action items:

**Batch 2 (Interviews 6-10):**
- Common pain point:
- Most requested feature:
- Biggest surprise:
- Action items:

---

## NPS Tracking (Net Promoter Score)

Ask users: "On a scale of 0-10, how likely are you to recommend [product] to a friend or colleague?"

### NPS Calculation
- **Promoters** (9-10): Loyal enthusiasts who will keep buying and refer others
- **Passives** (7-8): Satisfied but unenthusiastic -- vulnerable to competition
- **Detractors** (0-6): Unhappy users who can damage your brand through negative word-of-mouth
- **NPS = % Promoters - % Detractors** (ranges from -100 to +100)

### Monthly NPS Tracker

| Month | Responses | Promoters (9-10) | Passives (7-8) | Detractors (0-6) | NPS Score | Notes |
|---|---|---|---|---|---|---|
| January | 0 | 0 (0%) | 0 (0%) | 0 (0%) | -- | |
| February | 0 | 0 (0%) | 0 (0%) | 0 (0%) | -- | |
| March | 0 | 0 (0%) | 0 (0%) | 0 (0%) | -- | |
| April | 0 | 0 (0%) | 0 (0%) | 0 (0%) | -- | |
| May | 0 | 0 (0%) | 0 (0%) | 0 (0%) | -- | |
| June | 0 | 0 (0%) | 0 (0%) | 0 (0%) | -- | |
| July | 0 | 0 (0%) | 0 (0%) | 0 (0%) | -- | |
| August | 0 | 0 (0%) | 0 (0%) | 0 (0%) | -- | |
| September | 0 | 0 (0%) | 0 (0%) | 0 (0%) | -- | |
| October | 0 | 0 (0%) | 0 (0%) | 0 (0%) | -- | |
| November | 0 | 0 (0%) | 0 (0%) | 0 (0%) | -- | |
| December | 0 | 0 (0%) | 0 (0%) | 0 (0%) | -- | |

### NPS Follow-Up Questions

Always ask a follow-up question based on the score:

- **Promoters (9-10):** "What do you love most about [product]?" and "Would you be willing to leave a testimonial or review?"
- **Passives (7-8):** "What would we need to do to earn a 9 or 10 from you?"
- **Detractors (0-6):** "What's the primary reason for your score? What can we do to improve?"

### NPS Verbatim Responses

| Date | Score | Category | Verbatim Response | Action Taken |
|---|---|---|---|---|
| | | | | |
| | | | | |
| | | | | |

---

## Feedback Sources Checklist

Make sure you're collecting feedback from every channel:

- [ ] In-app feedback widget (e.g., Canny, Nolt, or custom)
- [ ] Email replies to onboarding and marketing emails
- [ ] Support ticket themes and patterns
- [ ] Social media mentions (Twitter, Reddit, Indie Hackers)
- [ ] App store reviews (if applicable)
- [ ] User interview program (aim for 2-4 per month)
- [ ] NPS survey (quarterly or bi-annually)
- [ ] Churn survey ("Why are you canceling?")
- [ ] Post-onboarding survey ("How was your setup experience?")
- [ ] Sales call objections log

---

## Common Feedback System Mistakes

### Mistake 1: Building Every Feature That's Requested
**What it looks like:** User requests dark mode. You build it. Another requests CSV export. You build it. Roadmap becomes a random wishlist.
**Why it fails:** You never say no. Product becomes bloated. You're reactive, not strategic.
**Fix:** Use RICE scoring. Only build features with RICE > 100 (or set your own threshold).

### Mistake 2: Only Talking to Power Users
**What it looks like:** You interview your 10 most active users. They all want advanced features.
**Why it fails:** Power users (5% of users) have different needs than the 95%. You over-index on complexity.
**Fix:** Interview across segments: churned users, free trial users, paying users, power users. Each group reveals different insights.

### Mistake 3: Asking "What features do you want?"
**What it looks like:** "What should we build next?" in a survey.
**Why it fails:** Users don't know what they want. They ask for faster horses, not cars.
**Fix:** Ask about **problems**, not solutions. "What's frustrating about your current workflow?" Then you design the solution.

### Mistake 4: Ignoring Churned Users
**What it looks like:** You only talk to happy, active customers.
**Why it fails:** Churned users know exactly why your product didn't work. That's gold.
**Fix:** Email every churned user within 48 hours: "We noticed you canceled. Can I ask why? 5-minute call?" Offer $25 gift card. 20% will respond.

### Mistake 5: Not Closing the Loop
**What it looks like:** User requests a feature. You build it. You never tell them.
**Why it fails:** They don't know you listened. They still think you're unresponsive.
**Fix:** When you ship a requested feature, email everyone who requested it: "You asked for [feature]. We built it. Here's how to use it."

### Mistake 6: Collecting Feedback But Never Acting
**What it looks like:** 100 feature requests in your tracker. None shipped in 6 months.
**Why it fails:** Users feel ignored. They stop giving feedback.
**Fix:** Ship at least 1 user-requested feature per month, even if small. Show you're listening.

### Mistake 7: Treating NPS as the Only Metric
**What it looks like:** "Our NPS is 50! We're doing great!" (But churn is 15% and nobody refers anyone.)
**Why it fails:** NPS measures sentiment, not behavior. People lie on surveys.
**Fix:** Track NPS + Churn + Referral Rate. Behavior > Sentiment.

### Mistake 8: Not Tagging Feedback by Customer Segment
**What it looks like:** You treat all feedback equally.
**Why it fails:** A $10/mo customer's feature request might not matter. A $500/mo customer's might be critical.
**Fix:** Tag feedback with customer tier (Free, Starter, Pro, Enterprise). Prioritize high-value segments.

### Mistake 9: Death by a Thousand Paper Cuts
**What it looks like:** You fix big bugs but ignore 20 small UX annoyances.
**Why it fails:** Small frustrations accumulate. Death by a thousand paper cuts. Users churn.
**Fix:** Every quarter, dedicate 1 week to "polish" - fixing the top 10 small annoyances. User satisfaction jumps.

### Mistake 10: Not Measuring Feature Adoption Post-Launch
**What it looks like:** You ship dark mode. You never check if anyone uses it.
**Why it fails:** You can't learn if the feature was worth it. You repeat the same prioritization mistakes.
**Fix:** Track feature usage in analytics. 30 days post-launch, check: What % of users adopted it? Did it improve retention? If <5% use it, you mis-prioritized.

---

## Feedback Collection Cadence (Monthly Rhythm)

**Week 1: Collect**
- Monday: Review all feedback from last week (support tickets, feature requests, bug reports)
- Wednesday: Send NPS survey to 10% of active users (rotate cohorts monthly)
- Friday: Reach out to 2-3 users for interviews (aim for 8-10 interviews/month)

**Week 2: Synthesize**
- Monday: Update Feature Requests table with RICE scores
- Wednesday: Tag bugs by severity, assign owners
- Friday: Write "Top 5 Insights from Interviews" summary doc

**Week 3: Decide**
- Monday: Roadmap planning meeting. Use RICE scores to pick top 3 features for next month.
- Wednesday: Design/spec the top priority feature
- Friday: Share roadmap update with team and key customers

**Week 4: Close the Loop**
- Monday: Ship 1 user-requested feature (even if small)
- Wednesday: Email everyone who requested that feature
- Friday: Publish changelog and share on social media

**Repeat monthly.**

---

## Recommended Tools for Feedback Management

**Feature Request Tracking:**
- **Canny** ($50/mo) - Public roadmap + voting + changelog. Great for transparency.
- **Nolt** ($25/mo) - Similar to Canny, cheaper for small teams.
- **Linear** (Free for <10 users) - If you want feedback + dev tasks in one place.
- **Notion** (Free) - Use this template! Free, flexible, full control.

**User Interviews:**
- **Calendly** (Free) - Let users book interview slots
- **Zoom** (Free) - Record interviews
- **Otter.ai** ($10/mo) - Auto-transcribe interviews, searchable

**NPS Surveys:**
- **Canny** (includes NPS feature)
- **Postmark** (Free NPS email templates)
- **Typeform** ($25/mo) - Beautiful surveys, high completion rate

**Bug Tracking:**
- **Linear** (Free for small teams) - Fast, beautiful, keyboard-first
- **GitHub Issues** (Free) - If you're already on GitHub
- **Notion** (Free) - Use this template!

**Analytics (Feature Adoption):**
- **PostHog** (Free tier: 1M events/mo) - Open-source product analytics
- **Mixpanel** (Free tier: 20M events/mo) - Feature usage tracking
- **Plausible** ($9/mo) - Privacy-friendly web analytics

---

> **Final Tip:** Review this entire feedback system every two weeks. Look for patterns across feature requests, bug reports, interviews, and NPS data. The signal is in the overlap -- when multiple channels point to the same problem, that's your highest-leverage thing to fix. Don't build in a vacuum. The best indie hackers spend 20% of their time building and 80% of their time listening to users, synthesizing feedback, and making smart bets on what to build next.
