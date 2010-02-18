## gitopen

Gitopen is a script that will open your most recently edited files from a Git repository in your $EDITOR.

First it checks is there are any modified (staged or unstaged) or untracked files (that aren't .gitignored) and opens those.

If there are none, then it searches for the last commit authored by $(git config --get user.email) and opens the files contained in that commit.

If you haven't yet authored a commit in the current repository, it will open all files in the most recent commit regardless of author.

## dependencies

Gitopen is a Ruby script and thus requires Ruby to be installed.  It also invokes the following system commands:

- file
- awk

and of course, '''git'''.
