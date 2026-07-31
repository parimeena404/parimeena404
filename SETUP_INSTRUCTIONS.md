# 🚀 Profile Setup & Installation Instructions

Follow these exact steps to deploy your new premium GitHub profile. 

## 1. Prepare the Repository
If you haven't already, ensure your profile repository (`parimeena404/parimeena404`) is set to **Public**.

## 2. Copy the Files
Copy the contents of this folder directly into the root of your repository:
- `README.md`
- `assets/` folder
- `.github/` folder

## 3. Enable GitHub Actions
The dynamic snake animation and metrics require GitHub Actions to run.
1. Go to the **Actions** tab in your repository.
2. Click **"I understand my workflows, go ahead and enable them"**.
3. You will see two workflows: **Generate Snake** and **Metrics**.
4. You can run them manually by clicking on them on the left sidebar, clicking **Run workflow**, and selecting the `main` branch.

## 4. Set Up the Snake Action Output Branch
The snake animation generates SVG files and pushes them to a branch named `output`.
1. The first time the Action runs, it will create the `output` branch automatically.
2. Ensure you have given GitHub Actions write permissions:
   - Go to **Settings** > **Actions** > **General**.
   - Under **Workflow permissions**, select **"Read and write permissions"** and click Save.

## 5. Set Up the Metrics Token
The advanced metrics workflow needs a GitHub token to fetch your stats.
1. Go to your GitHub **Settings** (top right dropdown) -> **Developer settings** -> **Personal access tokens** -> **Tokens (classic)**.
2. Generate a new token with the following scopes:
   - `repo`
   - `read:user`
   - `read:org`
3. Copy the generated token.
4. Go to your `parimeena404` repository **Settings** -> **Secrets and variables** -> **Actions**.
5. Click **New repository secret**.
6. Name it `METRICS_TOKEN` and paste your copied token into the value field. Save it.

## 6. Update Dynamic Data
- Replace `mailto:parimeena@example.com` in `README.md` with your actual email address.
- Add your actual links to Instagram and X (Twitter) in the social badges section.
- You can change the "Currently Building" and "Exploring" text directly in the `README.md` file whenever you start a new project.

## 7. Generating Assets with AI
Check the `PROMPTS.md` file for exact instructions on how to generate a custom logo and project banners using Midjourney or DALL-E 3.

## 8. Commit and Push
Once everything is copied and configured:
```bash
git add .
git commit -m "feat: upgrade github profile to premium tier"
git push origin main
```
Enjoy your world-class GitHub profile!
