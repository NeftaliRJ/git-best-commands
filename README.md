Git Commands
============

_A list of useful commands of git_

*The purpose of this repository is to collect the most practical git commands that I have come across, feel free to use them and combine them with Git Aliases to improve their practicality.*

--

### Clone projects

| Command | Description |
| ------- | ----------- |
| `git remote set-url origin ssh://git@github.com/[username]/[repository-name].git` | Set a repository's origin branch to SSH |
| `git remote add origin ssh://git@github.com/[username]/[repository-name].git` | Add a remote repository |

### Logs 

| Command | Description |
| ------- | ----------- |
| `git log --oneline --decorate --graph` | View of logs in a better way |
| `git log --diff-filter=D --summary` | Show deleted files in the history |
| `git log --all --online --grep 'word-to-search'` | Look specific word in all history |
| `git show --name-status --diff-filter=A <hash>` | List of files added to a commit |

### General

| Command | Description |
| ------- | ----------- |
| `git diff --color-words='\''\w+|.' ` | View diff by highlighting colors |
| `git diff > [name-file].patch` | Save diffs in file |
| `git apply [name-file].patch` | Apply diffs of the file in repo |
| `git commit --amend --no-edit` | Keep commit messages and add new file changes |
| `git commit --amend -m ‘new message’` | Modify the last commit in the branch |
| `git stash branch new-branch-name stash@{N}` | Create new brach with specific index |
| `git shortlog -sn` | Count the total commits by developer |
| `git shortlog -sn --all --no-merge ` | Count the total commits by developer without merges|
| `git blame [File-path]` | Show the changes line by line of file |
