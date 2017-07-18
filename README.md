A collection of [git hooks](https://git-scm.com/book/gr/v2/Customizing-Git-Git-Hooks) of possible utility.  (I optimistically created a repo to hold multiple hooks despite having only written one.)

## Hooks

### rubocop-pre-commit

A pre-commit hook that aborts commits containing style violations.

```shell
bschmeck@osprey
[master] ~/src/example_repo > git ci -m "Example for a blog post"
Running rubocop against spec/example_repo/example_spec.rb
Rubocop found 13 offenses.  Aborting commit.
spec/example_repo/example_spec.rb:9 Metrics/LineLength: Line is too long. [125/100]
```

#### Installation

1. Clone this repo
2. Symlink the `rubocop-pre-commit` script to `pre-commit` in the `.git/hooks` directory of the desired repo(s)
3. Ensure the `pre-commit` file is executable
