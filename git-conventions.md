# Git conventions

## Naming the branches

- **Feature branches**: `feature/<name>` or `feat/<name>` the branches for new features
- **Bugfix branches**: `bugfix/<name>` or `fix/<name>` the branches for bug fixes
- **Hotfix branches**: `hotfix/<name>` or `hf/<name>` the branches for urgent bug fixes
- **Release branches**: `release/<version>` or `rel/<version>` the branches for preparing a new release
- **Chore branches**: `chore/<name>` or `ch/<name>` the branches for maintenance tasks for example upgrade a package


## Commit messages

- **Feature commits**: `feat: <description>` the commit messages for new features
- **Bugfix commits**: `fix: <description>` the commit messages for bug fixes
- **Hotfix commits**: `hf: <description>` the commit messages for urgent bug fixes
- **Release commits**: `rel: <description>` the commit messages for preparing a new release
- **Chore commits**: `ch: <description>` the commit messages for maintenance tasks for example upgrade a package

Usually, the commit messages should be in the present tense and start with a verb. For example:
- `feat: add new feature`
- `fix: fix bug`
- `hf: fix urgent bug`
- `rel: prepare release`
- `ch: upgrade package`

Also we want to keep the commit messages with this command:

```
git commit
```

Without the `-m` flag because we want to use a title and a body


