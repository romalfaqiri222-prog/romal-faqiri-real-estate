# Faqiri Real Estate Afghanistan

Afghanistan real-estate marketplace and CRM platform in Dari RTL, backed by Supabase.

## Production

Current live URL: https://romal-faqiri-real-estate.onrender.com/

Target domain: https://www.faqirirealestate.af/

## Stack

- Static HTML/CSS/JavaScript frontend
- Supabase Auth, Postgres, Storage and Row Level Security
- Render Static Site hosting
- Progressive Web App (manifest + service worker)
- Metricool-connected social publishing

## Main workflows

- Public property search and property details
- User authentication and profiles
- Property submission with moderated publishing
- Property media uploads
- Favorites and saved searches
- Offers, inquiries and viewing requests
- Agent CRM
- Verification requests for identity, licensed office and property
- Admin moderation, reports, verification review and audit logs

## Security

- RLS enabled on exposed public tables
- Private verification documents
- Privileged profile, agency and property fields protected at database level
- Admin helper functions kept outside the exposed public schema
- Static-site security headers configured in Render
- Supabase browser client pinned to a specific version

## Remaining production handoff

1. Connect faqirirealestate.af and www.faqirirealestate.af in Render and DNS.
2. After the custom domain is live, update robots.txt and sitemap.xml to the official domain.
3. Configure romal@faqirirealestate.af with the selected email provider and add MX/SPF/DKIM/DMARC records.
4. Enable Supabase Auth leaked-password protection in the Supabase Dashboard.
5. Run final authenticated browser QA with a normal user and an admin account.
