# How To Update Tags
- make some changes and commit them
- `git tag -d 1.0` (removes tag from wherever it was before)
- `git tag 1.0` (adds `1.0` tag to your current `HEAD`)
- `git rev-parse HEAD` (shows your current commit sha, which will be useful in the next step)
- `git rev-list -n 1 1.0` (shows the commit sha associated with your tag, which is nice for a quick manual verification that things are cool)
- `git push origin <branch_name>` (pushes **ONLY** your commit to `<branch_name>`)
- `git push origin --tags --force` (force-pushes your tag changes to your remote, which effectively "moves" them from where they were to where they currently are)
