# SaaS Launch Checklist

> Your complete pre-launch, launch day, and post-launch checklist. Duplicate this page and check items off as you go.

---

## Pre-Launch

### Domain & Hosting

- [ ] Purchase primary domain name
- [ ] Set up DNS records (A, CNAME, MX)
- [ ] Configure SSL/TLS certificate (HTTPS)
- [ ] Choose and provision hosting provider (Vercel, Railway, Fly.io, etc.)
- [ ] Set up staging environment
- [ ] Set up production environment
- [ ] Configure CDN for static assets
- [ ] Set up custom email domain (e.g., hello@yoursaas.com)

### Legal

- [ ] Register business entity (LLC, sole proprietorship, etc.)
- [ ] Obtain EIN / tax identification number
- [ ] Set up business bank account
- [ ] Draft and publish **Privacy Policy**
- [ ] Draft and publish **Terms of Service**
- [ ] Draft and publish **Cookie Policy** (if applicable)
- [ ] Add GDPR compliance measures (if serving EU users)
- [ ] Add CCPA compliance measures (if serving CA users)
- [ ] Set up a DPA (Data Processing Agreement) template
- [ ] Confirm compliance with payment processor requirements

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

> **Tip:** Duplicate this page for each product launch. Not every item applies to every SaaS -- delete what you don't need and add what's unique to your product.
