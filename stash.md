## Why: Problem solved
#### Scenario:
  - 🏃‍♀️ I'm halfway working on `MyFeature` branch
  - ⛑️ My collegue comes, asking for help
  - 💱 I have to switch to `Master` branch, but don't want commit my work

#### Solution
- Save unsaved changes to stash (like stack)
```console
git stash
```
- Pop those changes out of stash merge to current branch
```console
git stash pop
```
- Merge what's in stash to current branch, but it remains in stash (for other branch)
```console
git stash apply
```
