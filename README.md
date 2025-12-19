# danger-spike-ci

Spike repository for testing Danger Swift with Fake CI mode.

## Key Feature: Fake CI Mode

This spike tests the `DANGER_FAKE_CI` approach where:
1. Workflows are triggered by `push` (not `pull_request: synchronize`)
2. PR is discovered via GitHub API
3. Danger posts comments using Fake CI mode

This avoids duplicate workflow runs while still updating Danger comments on every push.

## Tags

- `actions/ios/danger/v1` - iOS Danger action with Fake CI
- `workflows/ios/feature/v1` - Feature CI workflow
