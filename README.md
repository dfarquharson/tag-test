# How To Update Tags
- make some changes and commit them
- `git tag -d 1.0` (removes tag from wherever it was before)
- `git tag 1.0` (adds `1.0` tag to your current `HEAD`)
- `git push origin <branch_name>` (pushes **ONLY** your commit to `<branch_name>`)
- `git push origin --tags --force` (force-pushes your tag changes to your remote, which effectively "moves" them from where they were to where they currently are)
