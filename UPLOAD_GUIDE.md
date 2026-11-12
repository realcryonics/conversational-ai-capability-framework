# GitHub upload guide (private first)

The connected GitHub integration used to prepare this package can edit existing repositories but cannot create a new repository. No new GitHub repository has been created automatically.

1. Sign into GitHub and create a **private** repository named `conversational-ai-capability-framework` (do not pre-initialize with a README if uploading via command line).
2. Extract the ZIP and open a terminal in the extracted `conversational-ai-capability-framework` directory.
3. Run:

```bash
git init
git add .
git commit -m "Initial research draft: LV0-LV6 capability taxonomy"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/conversational-ai-capability-framework.git
git push -u origin main
```

Replace `YOUR_USERNAME` with your account name. Alternatively, upload these files via GitHub's **Add file → Upload files** in the empty private repo, preserving folders.

4. Review `research/limitations.md` and rights/permissions before changing repository visibility to public or adding a license.
