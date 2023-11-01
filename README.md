## Create pre-commit hook
$ touch .git/hooks/pre-commit

$ chmod +x .git/hooks/pre-commit

```#!/bin/sh
cat .git/hooks/pre-commit

# Run linting tool
flake8 .
```

## Coding flow

### Before add code to staging area

Should be run to check lint & format by command

```
$ make lint

$ make format
```


### Before commit code to repository

Using pre-commit git hooks to automate code checks

If pre-commit hook failed, you can commit code to repository.

