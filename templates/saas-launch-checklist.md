# SaaS Launch Checklist

> Your complete pre-launch, launch day, and post-launch checklist. Duplicate this page and check items off as you go.

---

## How This Checklist Works (Read This First)

This is a 120+ item checklist based on successful SaaS launches. Not every item applies to every product.

**Key:**
- 🔴 **Critical** - Must do. Product won't work or you'll face legal/security issues without this.
- 🟡 **Important** - Should do. Skipping this will hurt growth or user experience.
- 🟢 **Nice to Have** - Optional. Do if you have time, skip if you're rushing to launch.
- ⏱️ **Time estimate** - How long this typically takes

**Strategy:** Do all 🔴 items first. Then 🟡 items. Then 🟢 if time allows.

**Common Mistake:** Trying to do everything perfectly before launch. Ship with the 🔴 items done, iterate on 🟡 and 🟢 post-launch.

---

## Pre-Launch

### Domain & Hosting

- [ ] 🔴 Purchase primary domain name (⏱️ 10 min, $10-15/year)
- [ ] 🔴 Set up DNS records (A, CNAME, MX) (⏱️ 15 min) - Skip if using Vercel (auto-configured)
- [ ] 🔴 Configure SSL/TLS certificate (HTTPS) (⏱️ 5 min, usually auto with host)
- [ ] 🔴 Choose and provision hosting provider (Vercel, Railway, Fly.io, etc.) (⏱️ 30 min)
- [ ] 🟡 Set up staging environment (⏱️ 20 min) - Skip if solo founder, just use feature branches
- [ ] 🔴 Set up production environment (⏱️ 30 min)
- [ ] 🟢 Configure CDN for static assets (⏱️ 1 hour) - Skip if using Vercel/Cloudflare (built-in)
- [ ] 🟡 Set up custom email domain (e.g., hello@yoursaas.com) (⏱️ 30 min, $0-6/mo)

### Legal

- [ ] 🟡 Register business entity (LLC, sole proprietorship, etc.) (⏱️ 2-4 hours, $50-500) - Skip if pre-revenue, operate as sole prop
- [ ] 🟡 Obtain EIN / tax identification number (⏱️ 15 min, free) - Skip if not US-based
- [ ] 🟡 Set up business bank account (⏱️ 1 hour) - Skip until first $1k revenue
- [ ] 🔴 Draft and publish **Privacy Policy** (⏱️ 1 hour, free with generator) - Use Termly.io or TermsFeed
- [ ] 🔴 Draft and publish **Terms of Service** (⏱️ 1 hour, free with generator) - Use Termly.io or TermsFeed
- [ ] 🟢 Draft and publish **Cookie Policy** (⏱️ 30 min) - Skip if not using tracking cookies beyond analytics
- [ ] 🟡 Add GDPR compliance measures (⏱️ 2 hours) - Skip if not serving EU users (but you probably are)
- [ ] 🟢 Add CCPA compliance measures (⏱️ 1 hour) - Skip if <$25M revenue or not targeting CA users
- [ ] 🟢 Set up a DPA (Data Processing Agreement) template (⏱️ 30 min) - Skip until enterprise customers ask for it
- [ ] 🔴 Confirm compliance with payment processor requirements (⏱️ 30 min) - Stripe requires ToS + Privacy Policy links

### Branding

- [ ] Finalize product name and tagline
- [ ] Design logo (primary + favicon)
- [ ] Define brand colors and typography
- [ ] Create Open Graph / social sharing images
- [ ] Prepare press kit (logo files, founder headshot, boilerplate)

---

## Technical

### Authentication & Security

- [ ] Implement user sign-up flow (email/password or magic link)
- [ ] Implement user login flow
- [ ] Implement password reset / forgot password
- [ ] Add OAuth providers (Google, GitHub, etc.) if needed
- [ ] Implement email verification
- [ ] Set up rate limiting on auth endpoints
- [ ] Configure CORS properly
- [ ] Run basic security audit (SQL injection, XSS, CSRF)
- [ ] Set up two-factor authentication (optional, recommended)

### Payments & Billing

- [ ] Integrate payment processor (Stripe, Lemon Squeezy, Paddle)
- [ ] Create subscription plans / pricing tiers
- [ ] Implement free trial flow (if applicable)
- [ ] Implement upgrade / downgrade flow
- [ ] Implement cancellation flow
- [ ] Set up webhook handlers for payment events
- [ ] Test billing in sandbox / test mode
- [ ] Handle failed payments and dunning emails
- [ ] Generate and send invoices / receipts
- [ ] Set up tax collection (Stripe Tax, etc.)

### Transactional Email

- [ ] Choose email provider (Resend, Postmark, SendGrid, SES)
- [ ] Set up welcome email
- [ ] Set up email verification email
- [ ] Set up password reset email
- [ ] Set up payment receipt / invoice email
- [ ] Set up trial expiring reminder email
- [ ] Set up cancellation confirmation email
- [ ] Test email deliverability (check spam scores)
- [ ] Configure SPF, DKIM, and DMARC records

### Analytics & Monitoring

- [ ] Set up product analytics (PostHog, Mixpanel, Plausible, etc.)
- [ ] Set up website analytics (Plausible, Fathom, or GA4)
- [ ] Define key events to track (sign-up, activation, conversion, churn)
- [ ] Set up error tracking (Sentry, BugSnag)
- [ ] Set up uptime monitoring (BetterStack, UptimeRobot)
- [ ] Set up server/application logging
- [ ] Set up alerting for critical errors and downtime
- [ ] Create a basic analytics dashboard

### SEO & Performance

- [ ] Add meta titles and descriptions to all public pages
- [ ] Add Open Graph and Twitter Card meta tags
- [ ] Create and submit sitemap.xml
- [ ] Create robots.txt
- [ ] Add structured data / JSON-LD where appropriate
- [ ] Optimize page load speed (target < 3s)
- [ ] Optimize images (WebP, lazy loading)
- [ ] Test Core Web Vitals (LCP, FID, CLS)
- [ ] Set up Google Search Console
- [ ] Set up Bing Webmaster Tools (optional)

---

## Marketing

### Landing Page

- [ ] Write compelling headline and subheadline
- [ ] Write clear value proposition (3-5 bullet points)
- [ ] Add product screenshots or demo video/GIF
- [ ] Add social proof (testimonials, logos, user count)
- [ ] Add pricing section
- [ ] Add FAQ section
- [ ] Add clear call-to-action (CTA) buttons
- [ ] Optimize landing page for mobile
- [ ] A/B test headline or CTA (optional)
- [ ] Set up conversion tracking on CTA clicks

### Social Profiles

- [ ] Create Twitter/X account for product
- [ ] Create LinkedIn page (if B2B)
- [ ] Set up Product Hunt upcoming page
- [ ] Create Indie Hackers product page
- [ ] Claim relevant subreddit flair / community profiles
- [ ] Prepare branded social media banners

### Email List & Audience

- [ ] Set up email marketing tool (ConvertKit, Buttondown, Loops)
- [ ] Create a waitlist or early access landing page
- [ ] Write a 3-5 email welcome sequence
- [ ] Build an audience of at least 100 people before launch
- [ ] Prepare launch announcement email draft
- [ ] Segment list: waitlist vs. beta users vs. customers

### Pre-Launch Buzz

- [ ] Build in public: share progress on Twitter/X
- [ ] Write 2-3 blog posts about the problem you solve
- [ ] Engage in relevant communities (Reddit, IH, Discord, Slack)
- [ ] Reach out to 10-20 potential beta testers
- [ ] Collect and incorporate beta feedback
- [ ] Line up 3-5 testimonials or case studies from beta users

---

## Launch Day

### Directory Submissions

- [ ] Submit to Product Hunt (schedule at 12:01 AM PT)
- [ ] Post on Hacker News (Show HN)
- [ ] Post on Indie Hackers
- [ ] Post on relevant subreddits (r/SaaS, r/startups, r/entrepreneur, niche subs)
- [ ] Submit to BetaList
- [ ] Submit to SaaSHub
- [ ] Submit to AlternativeTo
- [ ] Submit to ToolFinder / There's An AI For That (if AI-related)
- [ ] Submit to relevant niche directories

### Social & Community

- [ ] Publish launch tweet/thread on Twitter/X
- [ ] Post launch announcement on LinkedIn
- [ ] Share in relevant Discord servers
- [ ] Share in relevant Slack communities
- [ ] Share in relevant Facebook groups
- [ ] DM warm contacts and ask for support / upvotes
- [ ] Reply to every comment and question within 1 hour

### Email

- [ ] Send launch announcement to full email list
- [ ] Send personal emails to beta users and supporters
- [ ] Send personal emails to potential partners / affiliates

### Monitor

- [ ] Monitor uptime and error rates closely
- [ ] Watch server resource usage (CPU, memory, DB connections)
- [ ] Monitor payment processing for issues
- [ ] Track real-time analytics (sign-ups, conversions)
- [ ] Keep a log of bugs reported on launch day
- [ ] Have a rollback plan ready if critical issues arise

---

## Post-Launch (Week 1-4)

### Feedback & Iteration

- [ ] Set up a feedback collection channel (Canny, feedback form, email)
- [ ] Reach out to first 10 paying customers for a quick call
- [ ] Categorize feedback: bugs, feature requests, UX issues
- [ ] Fix critical bugs within 24-48 hours
- [ ] Prioritize top 3 feature requests for next iteration
- [ ] Ship first post-launch update and announce it
- [ ] Send a "What's New" email to users

### Metrics & Growth

- [ ] Track MRR (Monthly Recurring Revenue) daily
- [ ] Track churn rate weekly
- [ ] Calculate CAC (Customer Acquisition Cost)
- [ ] Calculate LTV (Lifetime Value)
- [ ] Track activation rate (sign-up to first key action)
- [ ] Track conversion rate (free to paid)
- [ ] Identify top acquisition channels
- [ ] Set monthly growth targets
- [ ] Set up a weekly metrics review habit (every Monday)

### Content & SEO

- [ ] Publish a "lessons learned from launch" blog post
- [ ] Write 2-4 SEO-targeted articles in month one
- [ ] Start a changelog (public or email-based)
- [ ] Create 1-2 tutorial / how-to content pieces
- [ ] Repurpose blog content into Twitter threads and LinkedIn posts

### Sustainability

- [ ] Set up automated billing alerts and revenue notifications
- [ ] Document key processes (deploy, support, onboarding)
- [ ] Set up a support system (help desk, knowledge base, or email)
- [ ] Create onboarding email sequence for new sign-ups
- [ ] Plan roadmap for the next 90 days

---

## Launch Readiness Self-Assessment

Before you launch, answer these honestly:

**Product Readiness:**
- [ ] Can a new user sign up and get value in <10 minutes without my help?
- [ ] Have at least 5 people used the product and NOT asked "how does this work?"
- [ ] Is the core workflow bug-free? (Not perfect, but not broken)

**Market Readiness:**
- [ ] Have I talked to 20+ people in my target market about their problem?
- [ ] Do at least 10 people know my product exists and are waiting for launch?
- [ ] Can I articulate the problem I solve in one sentence?

**Business Readiness:**
- [ ] Is payment processing working? (Test mode purchases successful?)
- [ ] Do I have 4+ hours on launch day to respond to feedback and fix urgent issues?
- [ ] Have I written down what success looks like? (10 sign-ups? 2 customers? 100 upvotes?)

If you answered "No" to more than 2 questions, delay your launch. Fix those gaps first.

---

## Common Launch Mistakes (Learn from Others' Pain)

### Mistake 1: Launching Too Early (MVP is Too M)
**What it looks like:** Product is so bare-bones that users sign up and immediately churn.
**Cost:** You burn your one chance at a first impression. Users won't come back.
**Fix:** Launch when the product delivers the core value promise, even if it's ugly or missing nice-to-haves.

### Mistake 2: Launching Too Late (Perfectionism)
**What it looks like:** You spend 12 months building features nobody asked for.
**Cost:** Opportunity cost. Competitor launches in month 3 and captures the market.
**Fix:** Launch when 5 beta users can successfully use the product without hand-holding.

### Mistake 3: No Pre-Launch Audience
**What it looks like:** You build in silence for 6 months, then launch to 0 followers and crickets.
**Cost:** No initial momentum. Launch day feels like a failure. You get demoralized.
**Fix:** Build in public for 4-8 weeks before launch. Grow to 100+ followers. Build a waitlist.

### Mistake 4: Launching on Friday or Weekend
**What it looks like:** You submit to Product Hunt on Friday afternoon.
**Cost:** Lower traffic Fri-Sun. You miss the peak engagement window. Plus, if something breaks, you're firefighting on Saturday.
**Fix:** Launch Tuesday-Thursday. Ideally Tuesday or Wednesday at 12:01 AM PT.

### Mistake 5: No Launch Plan (Just "Winging It")
**What it looks like:** You wake up on launch day and think "Okay, I'll post on Reddit I guess?"
**Cost:** Scattered energy. You forget platforms. You miss the momentum.
**Fix:** Use this checklist. Prepare posts 48 hours before launch. Schedule them.

### Mistake 6: Ignoring Product Hunt Rules
**What it looks like:** You ask friends to upvote. PH detects it. You get shadowbanned.
**Cost:** Your launch gets buried or removed. Permanent reputation hit.
**Fix:** Read PH community guidelines. No vote manipulation. Genuine outreach only.

### Mistake 7: Not Responding to Feedback Fast
**What it looks like:** People comment on your PH/HN/Reddit post. You reply 8 hours later.
**Cost:** Algorithms punish slow response. Your post drops in rankings. Users feel ignored.
**Fix:** Block your entire launch day calendar. Respond to every comment within 15-30 minutes.

### Mistake 8: Defensive Responses to Criticism
**What it looks like:** Someone says "This is too expensive." You reply "Well, actually, our competitor charges more..."
**Cost:** You look insecure. Others pile on. Bad vibes kill momentum.
**Fix:** Thank critics. "Thanks for the feedback! Can you share what price would feel fair to you?" You learn + look gracious.

### Mistake 9: No Follow-Up After Launch
**What it looks like:** You get 50 sign-ups on launch day, then never email them again.
**Cost:** 90% of them forget you exist. You had their attention and wasted it.
**Fix:** Email every launch day sign-up within 24 hours. "Thanks for trying [product]. Here's how to get the most value..."

### Mistake 10: Measuring Success by Vanity Metrics
**What it looks like:** "We got 500 upvotes!" (But 2 paying customers and 50% of users churned in week 1.)
**Cost:** False sense of success. You don't fix the real problems (product, onboarding, pricing).
**Fix:** Define success as: X paying customers OR Y qualified leads OR Z trial users who complete onboarding.

---

## Launch Day War Room Checklist

On launch day, you need these tabs open:

- [ ] Product Hunt comments (reply to every comment within 15 min)
- [ ] Twitter mentions and DMs (reply to every mention)
- [ ] Reddit post comments (reply within 30 min)
- [ ] Indie Hackers post comments
- [ ] Hacker News post comments (if you posted there)
- [ ] Analytics dashboard (watch sign-ups in real-time)
- [ ] Error tracking tool (Sentry, BugSnag - catch bugs immediately)
- [ ] Stripe dashboard (watch for first payments)
- [ ] Email inbox (support requests)

**Pro tip:** Use a tool like Tweetdeck or Hootsuite to monitor all social mentions in one place.

**Energy management:** Launch day is a 12-14 hour marathon. Eat breakfast, have coffee ready, clear your calendar. This is your Super Bowl.

---

## Post-Launch: The First 48 Hours

The launch spike will fade. Here's how to sustain momentum:

**Hour 0-6 (Launch Morning):**
- Post everywhere simultaneously: PH, HN, Twitter, Reddit, IH, LinkedIn
- Pin your launch tweet
- DM 10-20 warm contacts: "Hey! I just launched [product]. Would love your support/feedback."
- Respond to every comment/question within 15 min

**Hour 6-12 (Launch Afternoon):**
- Check error logs. Fix critical bugs immediately.
- Send a "thank you" email to everyone who signed up in the first 6 hours
- Post an update thread on Twitter: "6 hours in. Here's what's happening..."
- Keep responding to comments

**Hour 12-24 (Launch Evening):**
- Triage feedback. Categorize: bugs, feature requests, confusion, praise
- Fix any critical UX issues (broken onboarding, confusing copy)
- Post a "Day 1 wrap-up" on Twitter/IH with stats: "X sign-ups, Y feedback items, Z bugs fixed"

**Hour 24-48 (Day 2):**
- Email launch day users who haven't activated yet: "Need help getting started?"
- Write a quick "lessons from launch day" post (do this while it's fresh)
- Reach out to any journalists or bloggers who covered similar products
- Plan your week 1 content: ship a quick feature based on top feedback

**Week 1 Goal:** Convert 20-30% of launch day sign-ups into activated users (completed core action). If that's not happening, onboarding is broken - fix it before running more marketing.

---

> **Final Tip:** Launch is not a one-time event. It's the start of a conversation. The real work begins after launch day - turning curious visitors into happy customers. Treat your first 100 users like gold. Talk to them. Fix their problems. They'll become your advocates and tell others. Word-of-mouth from those first 100 users will matter more than any launch spike.
