Carry Back setup

Important:
- If you want the /admin backend to update the website automatically, do NOT keep using manual Netlify ZIP uploads.
- Use GitHub + Netlify import. Then /admin edits commit changes to GitHub, and Netlify redeploys automatically.

Free stack:
- GitHub repo stores files
- Netlify deploys from GitHub automatically
- /admin uses Decap CMS to edit homepage, ticket content, product/request cards, and form trip/location options
- Interest form submissions go to Netlify Dashboard > Site > Forms > carryback-interest

Setup:
1. Create a GitHub repo, e.g. carry-back.
2. Upload all files/folders in this package to the repo root.
3. Netlify > Add new site > Import from GitHub > choose repo.
4. Build command: blank. Publish directory: .
5. In Netlify, keep Form Detection enabled.
6. Netlify > Identity > Enable Identity.
7. Identity > Services > Enable Git Gateway.
8. Invite yourself as user.
9. Open https://your-site.netlify.app/admin/ and log in.
10. Edit Homepage Settings to change the ticket/boarding-pass content and form trip/location options.

Form note:
- The HTML form already includes the required netlify attribute and hidden form-name field.
- The trip/location dropdown is controlled by Homepage Settings > Form trip / location options.
- Netlify detects forms at deploy time. If Forms still says “Add an HTML form...”, redeploy this package through the GitHub-connected Netlify site, then check Forms again.
