# Tabdeal APK Builder

This public repository contains only the build workflow. The application source remains in the private repository.

## One-time setup

1. Create a fine-grained GitHub personal access token with access only to `alisolimani3221-art/tabdeal-pro-bot` and **Contents: Read-only** permission.
2. In this repository, open **Settings → Secrets and variables → Actions → New repository secret**.
3. Add the secret named `PRIVATE_REPO_TOKEN` and paste the token value. Never commit or share the token.
4. Open **Actions → Build Tabdeal APK → Run workflow**.

The workflow checks out the private source, runs its tests, builds the Android APK, and uploads the APK as the `Tabdeal-Android-APK` artifact. Standard GitHub-hosted runners are free for public repositories.
