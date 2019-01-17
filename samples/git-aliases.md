# Using Azure DevOps CLI with Git

You can configure the Azure DevOps CLI to add git aliases for common git-based Azure DevOps CLI commands like creating or adding reviewers to pull requests.

## Configure the Azure DevOps CLI to add git aliases 

Run the `az devops configure` command with the `--use-git-aliases` flag set to `yes` to set up git aliases:

```
az devops configure --use-git-aliases yes
```

> After running the `az devops configure` command, you can test that it was successful by attempting to run `git pr create`, which should fail and ask you for an `--organization` flag.

## Example git alias commands

### Creating a pull request:

| Azure DevOps CLI Command                                    | git alias command                                                  |
| ----------------------------------------------------------- | ------------------------------------------------------------------ |
| az repos pr create --target-branch {branch\_name}           | git pr create --target-branch {branch\_name}                       |


### Add reviewers to a pull request:

| Azure DevOps CLI Command                                    | git alias command                                                  |
| ----------------------------------------------------------- | ------------------------------------------------------------------ |
| az repos pr reviewers add --id # --reviewers {name}         | git pr reviewers add --id # --reviewers {name}                     |

### Set a pull request to auto-complete:

| Azure DevOps CLI Command                                    | git alias command                                                  |
| ----------------------------------------------------------- | ------------------------------------------------------------------ |
| az repos pr update --id # --auto-complete on                | git pr update --id # --auto-complete on                            |
