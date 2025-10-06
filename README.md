# Reproduction  repo

This is a quick reproduction repo for semantic release issue [759](https://github.com/semantic-release/commit-analyzer/issues/759#issuecomment-3053396311)

Running `npx semantic-release -d` produces the following:

...
```
[10:26:33 PM] [semantic-release] [@semantic-release/commit-analyzer] › ℹ  Analyzing commit: fix: [XX-000] Removed npm plugin
[10:26:33 PM] [semantic-release] [@semantic-release/commit-analyzer] › ℹ  The release type for the commit is patch
[10:26:33 PM] [semantic-release] [@semantic-release/commit-analyzer] › ℹ  Analyzing commit: fix: [XX-000] Changes semantic config branch master to main
[10:26:33 PM] [semantic-release] [@semantic-release/commit-analyzer] › ℹ  The release type for the commit is patch
[10:26:33 PM] [semantic-release] [@semantic-release/commit-analyzer] › ℹ  Analyzing commit: feat!: [XX-000] Should trigger major
[10:26:33 PM] [semantic-release] [@semantic-release/commit-analyzer] › ℹ  The commit should not trigger a release
[10:26:33 PM] [semantic-release] [@semantic-release/commit-analyzer] › ℹ  Analyzing commit: Added gitignore. Fixed package.json
[10:26:33 PM] [semantic-release] [@semantic-release/commit-analyzer] › ℹ  The commit should not trigger a release
[10:26:33 PM] [semantic-release] [@semantic-release/commit-analyzer] › ℹ  Analyzing commit: Added semantic release config
[10:26:33 PM] [semantic-release] [@semantic-release/commit-analyzer] › ℹ  The commit should not trigger a release
[10:26:33 PM] [semantic-release] [@semantic-release/commit-analyzer] › ℹ  Analyzing commit: Initial commit
[10:26:33 PM] [semantic-release] [@semantic-release/commit-analyzer] › ℹ  The commit should not trigger a release
[10:26:33 PM] [semantic-release] [@semantic-release/commit-analyzer] › ℹ  Analysis of 6 commits complete: patch release
```

Point of interest:

`Analyzing commit: feat!: [XX-000] Should trigger major`

`The commit should not trigger a release`
