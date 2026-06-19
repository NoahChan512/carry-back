Carry Back setup

Use this folder for the Carry Back website, not Chronos Notes.

Free stack:
- GitHub repo stores files
- Netlify deploys the site
- /admin uses Decap CMS to edit products/settings
- Interest form submissions go to Netlify Dashboard > Forms > carryback-interest

Setup:
1. Create GitHub repo, e.g. carry-back
2. Upload all files/folders in this package.
3. Netlify > Add new site > Import from GitHub > choose repo.
4. Build command: blank. Publish directory: .
5. Netlify > Identity > Enable Identity.
6. Identity > Services > Enable Git Gateway.
7. Invite yourself as user.
8. Open https://your-site.netlify.app/admin/ and log in.
