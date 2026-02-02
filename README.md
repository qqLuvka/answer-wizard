<div align="center">
<img width="1200" height="475" alt="GHBanner" src="https://github.com/user-attachments/assets/0aa67016-6eaf-458a-adb2-6e31a0763ed6" />
</div>

# Run and deploy your AI Studio app

This contains everything you need to run your app locally.

View your app in AI Studio: https://ai.studio/apps/temp/1

## Run Locally

**Prerequisites:**  Node.js


1. Install dependencies:
   `npm install`
2. Set the `GEMINI_API_KEY` in [.env.local](.env.local) to your Gemini API key
3. Run the app:
   `npm run dev`


---

## Portable .exe for sharing (no install)

### Recommended: GitHub Actions (easiest)
1) Create a GitHub repo and push this project to `main`.
2) In GitHub: Settings → Secrets and variables → Actions → New repository secret:
   - Name: `GEMINI_API_KEY`
   - Value: your Gemini API key
3) Go to Actions → "Build Windows Portable EXE" → Run workflow.
4) Download the artifact `ReplyWizardAI-Portable-Windows` and share the `.exe` inside.

⚠️ Security note: embedding an API key into a desktop app means anyone with the .exe can potentially extract the key.
