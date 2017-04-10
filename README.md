A collection of [git hooks](https://git-scm.com/book/gr/v2/Customizing-Git-Git-Hooks) of possible utility.  (I optimistically created a repo to hold multiple hooks despite having only written one.) 

## Hooks

### rubocop-pre-commit

A pre-commit hook that aborts commits containing style violations.

#### Installation

1. Clone this repo 
2. Symlink the `rubocop-pre-commit` script to `pre-commit` in the `.git/hooks` directory of the desired repo(s)
3. Ensure the `pre-commit` file is executable
