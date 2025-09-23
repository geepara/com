# Deployment Setup Instructions

This repository uses GitHub Actions to automatically build and deploy the Hugo site to Netlify when code is pushed to the `prod` branch.

## Required GitHub Secrets

You need to add the following secrets to your GitHub repository:

### 1. NETLIFY_AUTH_TOKEN
- Go to [Netlify User Settings > Applications](https://app.netlify.com/user/applications)
- Under "Personal access tokens", click "New access token"
- Give it a name like "GitHub Actions Deploy"
- Copy the generated token
- Add it as `NETLIFY_AUTH_TOKEN` in your GitHub repository secrets

### 2. NETLIFY_SITE_ID
- Go to your Netlify site dashboard
- Go to Site settings > General
- Copy the "Site ID" (under Site details)
- Add it as `NETLIFY_SITE_ID` in your GitHub repository secrets

## How to Add Secrets to GitHub

1. Go to your GitHub repository
2. Click on "Settings" tab
3. In the left sidebar, click "Secrets and variables" > "Actions"
4. Click "New repository secret"
5. Add the secret name and value
6. Click "Add secret"

## How the Workflow Works

- Triggers on push to `prod` branch
- Checks out the code with submodules (for Hugo themes)
- Sets up Hugo with the latest version
- Builds the site with `hugo --minify`
- Deploys the `public` directory to Netlify
- Provides deployment status in commit comments

## Manual Deployment

If you need to manually trigger a deployment, push any change to the `prod` branch and the workflow will run automatically.
