# Vercel

## What is Vercel?

Basically a hosting platform

### What’s not included?

<div>

Things requiring server active > 1 minute:

- CMS - can use any CMS with an API
- Database - can hook to any database
- Email - can use any email service
- File uploads - can use headless CMS or file storage provider
- Cron jobs - can be called on a timer, though

</div>

_(most should be separate anyway)_

<Notes>

- CMS - only real notable change; has become increasingly separate over time
- Database - we typically advise these be separate anyway, so no big change here
- Email - should really be separate anyway, so no big change here
- File uploads - we typically either use the CMS or S3, so no big change here
- Cron jobs - are generally discouraged due to difficulty in documenting, requiring someone with both server and application knowledge to maintain, and usually being inefficient. We usually suggest things like web hooks instead.

</Notes>
## Who uses Vercel?

- Airbnb
- Auth0
- GitHub
- Hulu
- InVision
- McDonald’s
- Netflix
- Nike
- Tripadvisor
- Twilio
- Uber
- …

<Notes>

We want to use stable, high-quality tools created and used by the best teams in the industry

</Notes>
## Why are we adding this?

- focus on creating instead of hosting
- aligns better clients’ goals
- cheaper, faster, better experience, …

<Notes>

- we spend too much time setting up and maintaining instead of what we're good at
- clients generally don't want to spend money here, but we're still blamed if something bad happens - regardless of what agreements say

</Notes>
## Why should I care?
### Better workflow

#### Previous

- setup servers
- setup deployment
- develop
- launch to `develop`
- review
- launch to `staging`
- review with client
- launch to `production`

#### Next

- add project to Vercel
- develop
- preview
- switch to production

<Notes>

Mainly focusing on workflow for development and hosting

should require fewer people:

- setting up servers requires a specialist
- setting up deployments requires a specialist
- launching often requires a specialist

</Notes>

### Preview URLs

**Before:** Dev / Staging / Production<br />
**Now:** Preview URLs

URL for _every_ point of development

<Notes>

(example on next slide)

- one of my favorite features
- URL can be shared with anyone
- helps collaboration:
  - UX
  - AM
  - client
  - proofing

</Notes>
### Preview URLs - Example

- [version 1](https://christensenarms-selector-tool-cn7njmpu5-gsandf1.vercel.app/#WzAsMF0)
- [version 2](https://christensenarms-selector-tool-eqxdvabtg-gsandf1.vercel.app/#WzAsMF0)

[see all](https://vercel.com/gsandf/christensenarms-selector-tool)

<Notes>

- show how I was able to get feedback about wrapping card headers
- on "see all" - show preview, "Promote to Production", etc.

</Notes>
### “Serverless”

Very minimal configuration required

Handled for us:

- server security updates
- SSL/TLS certificates
- load balancing & auto-scaling
- push to deploy
- preview URLs in PRs

### Better performance

Handled for us:

- load balancing & auto-scaling
- serving using CDN
- caching (done right)
- asset compression

### Reduced costs

less time (setting up & maintaining)

$20/user/month with _very_ generous usage allowances

<Notes>

For comparison, in AWS, we'd get about 1-2 servers for that price.

That would NOT include:

- bandwidth
- server upgrades
- usage monitoring
- managing TLS certs
- setting up deployments (to server)

Also, in our AWS setup, we typically need 3 servers for 1 project. Just doing 1 project using Vercel, we start saving money.

</Notes>
## What projects will use Vercel?

✅ static sites<br />
✅ APIs without CMS<br />
❌ (for now) CMS sites: WordPress

### Why not CMS sites?

- need to figure out authoring flow
- most plugins wouldn’t work

In the future, we may choose a different CMS<br />
that works with us

# Questions?

# Thank You
