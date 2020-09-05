# Pre-commit hook for remark (markdown processor and linter)

This pre-commit hook allows you to run remark on git actions. For example autoformat and lint markdown files on each commit.

For pre-commit: see https://github.com/pre-commit/pre-commit

For remark-lint: see https://github.com/remarkjs/remark-lint


## Using remark with pre-commit

Add this to your `.pre-commit-config.yaml`:
```yaml

-   repo: https://github.com/MaratFM/pre-commit-remark
    rev: ''  # Use the sha or tag you want to point at
    hooks:
    -   id: remark
        args: [] # list of args for remark-lint
        additional_dependencies: ['remark-cli@8.0.1', 'remark-preset-lint-recommended@4.0.1'] # use latest version and add additional plugins here 
 ```
