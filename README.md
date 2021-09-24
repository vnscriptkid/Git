## This repo contains all you need to know about Git

#### To stop tracking a file you need to remove it from the index. This can be achieved with this command.
```console
git rm --cached <file>
```

#### Undo a reset
```console
git reflog
git reset be8e86f
```

#### Flow of working a new feature
```console
git checkout -b FixMessages
#### make lot of changes
git pull origin master
git push origin FixMessages
### asking boss to merge your branch to codebase
```

#### Merge branch `FixMessages` to `master`
```console
(master) git merge FixMessages
```

#### Reset one branch from whatever in remote right now
```console
git fetch --all
git branch backup-master
git reset --hard origin/master
```
