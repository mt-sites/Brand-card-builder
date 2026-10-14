TapLoop admin folder - what to do

1. Copy the "admin" folder (and the "_headers" file) into your EXISTING website folder,
   next to your other pages. Do not replace your whole site with this folder.
   Redeploy. The builder will be at:  your-site/admin/
2. In Cloudflare Zero Trust, create an Access application for that path only:
   hostname = your site, path = /admin   (keep your customer cards outside /admin so they stay public)
3. Add an Allow rule: Emails -> your own email. Sign-in method: One-time PIN.
4. Test /admin/ in a private window (sign-in code expected) and a customer card link (opens normally).
