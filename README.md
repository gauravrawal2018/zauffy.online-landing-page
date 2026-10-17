# zauffy.online domain acquisition listing

A lightweight, static landing page presenting **zauffy.online** as a domain available for acquisition. It uses HTML, CSS, and vanilla JavaScript, with no runtime, package manager, form backend, analytics, or tracking scripts.

## Preview locally with VS Code Live Server

1. Open this folder in Visual Studio Code.
2. Install the **Live Server** extension by Ritwick Dey if it is not already installed.
3. In the Explorer, right-click `index.html` and select **Open with Live Server**. Alternatively, click **Go Live** in the VS Code status bar.
4. Live Server opens the page in your browser. Changes to the HTML, CSS, or JavaScript will reload automatically.

The contact actions open the visitor's phone or email application. There is no inquiry form or message backend.

## Publish with GitHub Pages

1. Sign in to GitHub and create a new repository, for example `zauffy-domain`.
2. Keep the repository public for the simplest GitHub Pages setup, and do not initialize it with a README if you plan to push this existing folder.
3. In VS Code, open the terminal in this project folder and run:

   ```sh
   git init
   git add index.html css/style.css js/script.js assets/favicon.svg README.md .gitignore
   git commit -m "Build zauffy.online domain listing"
   git branch -M main
   git remote add origin https://github.com/YOUR-USERNAME/zauffy-domain.git
   git push -u origin main
   ```

   Replace `YOUR-USERNAME` with your GitHub username. If this folder is already a Git repository with a remote, use its existing repository setup instead of repeating `git init` or `git remote add`.
4. On GitHub, open the repository and go to **Settings → Pages**.
5. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/ (root)`, then save.
6. Wait for GitHub Pages to publish the site. The Pages settings show the generated `github.io` address and deployment status.

## Connect `zauffy.online`

1. In **Settings → Pages**, enter `zauffy.online` under **Custom domain** and save. GitHub will add a `CNAME` file to the publishing source.
2. At the domain registrar or DNS provider, configure the DNS records GitHub Pages currently recommends for a root domain. This commonly means apex `A` records for GitHub Pages and a `www` `CNAME` pointing to `<YOUR-USERNAME>.github.io`; use the values shown in GitHub's current Pages documentation and your Pages settings.
3. If you use `www.zauffy.online`, configure it as an additional custom domain or redirect it to the apex domain as appropriate. Avoid conflicting DNS records from existing hosting setups.
4. Allow DNS time to propagate. Once GitHub verifies the domain and the records are correct, return to **Settings → Pages** and enable **Enforce HTTPS** when that option becomes available.

This project has not been deployed, and no DNS changes have been made. GitHub Pages and DNS provider interfaces or recommended records may change, so follow the current values shown in your account.
