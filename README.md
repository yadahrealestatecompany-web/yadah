# yadahReviewing mobile project files so the publish workflow can target the correct Expo path.

Read [](file:///workspace/real-estate/apps/mobile)

Adding Expo/EAS publish workflow and mobile publish scripts for both local and CI publishing.

Replacing 24 lines with 26 lines in [](file:///workspace/real-estate/apps/mobile/package.json)

Read [](file:///workspace/real-estate/apps/mobile/package.json)

Read [](file:///workspace/real-estate/package.json)

Creating the mobile publish workflow and documenting the publish process.

Created [](file:///workspace/real-estate/.github/workflows/deploy-mobile.yml)

Read [](file:///workspace/real-estate/README.md)

Updating README to include the new mobile publish workflow and required Expo secret.

Replacing 14 lines with 30 lines in [](file:///workspace/real-estate/README.md)


```

```
## Mobile publish automation added

✅ Created `.github/workflows/deploy-mobile.yml`
- Builds/install deps
- Auths with Expo via `EXPO_TOKEN`
- Runs `pnpm --filter mobile publish`

✅ Updated README.md
- Documented mobile publish workflow
- Added required `EXPO_TOKEN` secret
- Included local publish command `pnpm publish:mobile`

### Notes
- `apps/mobile/package.json` already exposes `publish` via `expo publish --non-interactive --yes`
- You can now publish from GitHub by pushing `main` or using the workflow dispatch button in GitHub Actions

Made changes.
