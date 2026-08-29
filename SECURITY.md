# Security policy

## Reporting a vulnerability

**Please don't open a public issue for a security problem.** Use a
[private security advisory](https://github.com/Pup-Pup-Games/Sleddog-Feedback/security/advisories/new)
instead, or the [contact form](https://sleddog.tools/contact) if you'd rather not use GitHub.

A public report is a working exploit handed to everyone who reads it before we've
had a chance to ship a fix. A private one gives us that chance.

## What's in scope

Sled Dog is a hosted web app at **sleddog.tools**, backed by Supabase and
deployed on Vercel. Things we especially want to hear about:

- Access to another table's data — characters, parties, the steading, uploaded images
- Anything that bypasses the row-level security rules between accounts
- Authentication or session problems (magic link, Google, or Discord sign-in)
- Supporter/billing state that can be changed from the client
- Stored or reflected XSS, particularly anywhere user-authored content or
  community content is rendered

Out of scope: findings against `staging.sleddog.tools` (it's a deliberately open
test environment), volumetric denial of service, missing headers with no
demonstrated impact, and social-engineering the operator.

## What to expect

We're a very small studio, so please calibrate: you'll get a human reply, but not
an enterprise SLA.

- **Acknowledgement** within a few days.
- **An assessment** — whether we agree it's a vulnerability, and what we intend to
  do — within two weeks.
- **Credit** in the fix notes if you'd like it, or none at all if you'd prefer.

We don't run a paid bug bounty. We do genuinely appreciate the report, and we'll
say so publicly if you want us to.

## Please don't

Access, modify, or retain another person's data while testing. If a proof of
concept requires touching real user data, stop and describe the flaw instead —
we'll take your word for it.
