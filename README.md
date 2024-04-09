# Deploy Astro to GitHub Pages
Steps:

## GitHub Repositoy
Create a new GitHub repository

## 2. Astro Config
Add **Site** and **Base** to *astro.config.mjs* file
```js
export default defineConfig({
  ...
  site: 'https://yourGitHubName.github.io',
  base: '/repositoryName'
});
```

## 3. Workflow
- Create folder *.github*
- Inside *.github* create folder *workflows*
- Inside *workflows* create file *deploy.yml*
- Paste the YAML code given in this repo into this file

> .github/workflows/deploy.yml

## 4. Configure GitHub
In your repository:
- Go to *Settings* -> *Pages*
- Set *Source* as **GitHub Actions**
- Push your local repository to remote

> In *Actions* you will be able to get the URL of your site
