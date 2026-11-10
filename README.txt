DIL & DASTAAN - STATIC WEBSITE
Open index.html (or upload the whole folder to any static host).
Admin: /dd-admin-7f3k/  (default login admin / admin123 - change it in Account)

HOW EDITING WORKS (static site, no server):
1. Log in, edit, press Save -> you see changes on your own browser.
2. To publish for everyone: press "Download content.js" and replace assets/content.js on your host.

SECURITY - IMPORTANT:
A purely static site cannot truly hide a page. The login is client-side, so it only keeps casual visitors out.
To make /dd-admin-7f3k/ genuinely private, protect that folder at the host:
 - Cloudflare Pages: Zero Trust > Access policy on the path /dd-admin-7f3k/*
 - Netlify: password/visitor access or Identity role-based redirect for that path
 - Apache: use the included .htaccess with htpasswd (dd-admin-7f3k/.htaccess)
The page already has noindex so search engines skip it.
