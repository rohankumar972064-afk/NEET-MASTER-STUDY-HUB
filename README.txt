NEET Prep Hub — GitHub Pages + Auto Publish

FILES
- index.html
- admin.html
- questions.json
- quizzes.json

HOSTING
1. Create a GitHub repository.
2. Upload all files to the repository root.
3. Enable GitHub Pages from Settings > Pages > Deploy from branch > main > /(root).
4. Open your GitHub Pages URL.
5. Admin page: /admin.html

GITHUB AUTO-PUBLISH
The updated admin panel can publish questions.json and quizzes.json directly to GitHub using the GitHub REST Contents API.

SETUP TOKEN
1. GitHub > Settings > Developer settings > Personal access tokens > Fine-grained tokens.
2. Create a token and restrict it to ONLY the repository used by this website.
3. Repository permissions: Contents = Read and write.
4. Do not give unnecessary permissions.
5. Copy the token once and enter it in admin.html when publishing.

ADMIN WORKFLOW
1. Login to admin.html (demo credentials in the page; change the authentication before production).
2. Enter GitHub owner, repository, branch and token.
3. Test GitHub Connection.
4. Upload CSV/XLSX.
5. Validate and preview.
6. Click Publish to GitHub.
7. The admin updates questions.json and quizzes.json directly in the repository. GitHub Pages then deploys the changed static files.

IMPORTANT SECURITY NOTE
This is a static browser-based publisher. A GitHub write token entered into a browser is exposed to that browser/user. Do NOT put a token directly into HTML/JavaScript or share it with untrusted admins. For a public or multi-admin production system, use a backend or GitHub App/server-side token flow instead.

The GitHub API endpoint used is the repository Contents API. Updating an existing file requires its current blob SHA; the admin fetches the SHA and then updates the file serially.

COST
GitHub Pages and GitHub API access do not require a separate paid plan for this use case, subject to GitHub's current account/service limits and policies. A custom domain, if purchased, is separate.

ADS
Use ad placements that comply with your ad network policies. Never encourage users/admins to click ads or manipulate impressions/clicks.
