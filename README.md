# Career Path

Career Path is a simple, responsive college career-development website. It has three role-based demo portals in one page:

- **Sign-in page:** use the single Admin demo account.
- **Admin:** review the college member list, add demo teachers and students, and mark demo accounts active or inactive.
- Teacher and student profiles are sample records managed from the Admin demo; they do not have login accounts.
- Use **Sign out** to return to the sign-in page.

The site is plain HTML, CSS, and JavaScript in [`index.html`](./index.html). It has no package installation, build step, API key, or server requirement. Open `index.html` in a browser to try it. Demo edits are saved in that browser's local storage; clear this site's browser storage to restore all sample data.

## Admin demo sign-in

Use this single sample account:

| Role | Email | Password |
|---|---|---|
| Admin | `admin@college.edu` | `CareerPath@Admin2026!` |

The public sample credential is shown on the demo sign-in page. It is not real authentication.

## Important demo limitation

This is a front-end demonstration, not a secure student-information system. The admin demo sign-in only gates the visible page; it is not authorization, because its password is included in the public HTML. Sample member data is visible to anyone who can open the site, and browser-local changes are not shared with other users. Teacher and student sample profiles have no login credentials or separate sign-in. Do not enter real student information, passwords, or other sensitive data. Real accounts, invitations, role-based access controls, shared data, and private records require a server and database.

## Publish with GitHub Pages

1. Install Git if it is not already installed, then sign in to [GitHub](https://github.com/).
2. On GitHub, create a **new empty repository** named `career-path`. Do not add a README or license there if you already have these project files.
3. Open PowerShell in this project folder and replace `YOUR-GITHUB-USERNAME` with your GitHub username:

   ```powershell
   git init
   git add index.html README.md .gitignore
   git commit -m "Create Career Path college website"
   git branch -M main
   git remote add origin https://github.com/YOUR-GITHUB-USERNAME/career-path.git
   git push -u origin main
   ```

   If this folder is already a Git repository, skip `git init`. If `origin` is already configured, check it with `git remote -v` and update it only if it points to the wrong repository.

4. On the repository page, open **Settings → Pages**.
5. Under **Build and deployment**, choose **Deploy from a branch**, select branch **main** and folder **/(root)**, then click **Save**.
6. Wait for the Pages deployment to finish. Your site will be available at `https://YOUR-GITHUB-USERNAME.github.io/career-path/`.

The published page is the root `index.html`; GitHub Pages hosts it directly. No Node.js, Python, workflow, or hosting configuration is needed.

## Project files

- `index.html` — complete static Career Path demo website.
- `README.md` — project overview and GitHub Pages publishing guide.
