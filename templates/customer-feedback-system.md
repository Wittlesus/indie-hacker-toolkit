# Customer Feedback System

> A single source of truth for all customer feedback. Collect, organize, prioritize, and act on what your users are telling you.

---

## Feature Requests

Track every feature request in one place. Use the scoring system to prioritize what to build next.

### Scoring Guide

- **Votes:** How many unique users have requested this? (1 = one user, 5 = many users)
- **Effort:** How much work is this? (1 = trivial, 2 = small, 3 = medium, 4 = large, 5 = massive)
- **Impact:** How much value does this deliver? (1 = nice-to-have, 5 = game-changer)
- **Priority Score:** Impact x Votes / Effort (higher = build first)

| # | Feature Request | Requested By | Votes | Effort (1-5) | Impact (1-5) | Priority Score | Status | Target Date | Notes |
|---|---|---|---|---|---|---|---|---|---|
| 1 | Example: Dark mode | @user1, @user2 | 4 | 2 | 3 | 6.0 | Planned | Q1 | Popular request, relatively easy |
| 2 | Example: CSV export | @user3 | 2 | 3 | 4 | 2.7 | Under Review | -- | Important for power users |
| 3 | Example: Slack integration | @user4, @user5, @user6 | 5 | 4 | 5 | 6.3 | In Progress | Q2 | High impact but significant work |
| 4 | Example: Mobile app | @user7 | 1 | 5 | 3 | 0.6 | Backlog | -- | Low demand, very high effort |
| 5 | | | | | | | | | |
| 6 | | | | | | | | | |
| 7 | | | | | | | | | |
| 8 | | | | | | | | | |
| 9 | | | | | | | | | |
| 10 | | | | | | | | | |

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

### Interview Template

Before each interview, prepare these questions (customize to your product):

1. What made you sign up for [product]?
2. What problem were you trying to solve?
3. How were you solving this problem before [product]?
4. What's the most valuable thing [product] does for you?
5. What's the most frustrating thing about [product]?
6. If you could change one thing, what would it be?
7. Would you recommend [product] to a colleague? Why or why not?
8. How would you feel if you could no longer use [product]?

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

> **Tip:** Review this entire feedback system every two weeks. Look for patterns across feature requests, bug reports, interviews, and NPS data. The signal is in the overlap -- when multiple channels point to the same problem, that's your highest-leverage thing to fix.
