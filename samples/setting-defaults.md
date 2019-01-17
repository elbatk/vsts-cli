## Set up defaults and using Git defaults

Azure DevOps CLI supports setting up defaults like organization and project for ease of use. e.g.

```
az devops configure --defaults organization=https://dev.azure.com/myorganization  project=myproject
```

Default args will be used in any commands where these args are inputs but are not provided with the command.

Default values can be also detected from the Git remote url. If you are running a command from inside a Git repository folder, organization, project and repository name will be auto-detected from the Git remote url.

## Listing the defaults

You can list the defaults by running the following command:
```
az devops configure --list
```

## Using Git aliases

For more information on how to use Git aliases, refer to [Using Azure DevOps CLI with Git](git-aliases.md).

```
az devops configure --use-git-aliases yes
```
