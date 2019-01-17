# Opening an artifact in browser

You can use the `--open` flag to open any artifact in your default browser.

For example :
```
bash
az boards work-item show --id 1 --open 
```
This will show the details of work item with id 1 and also open it in the default browser.

# Auto-detect repository

By default, the detect flag is on for every command.
So, if your current working directory is a Git repository, the Azure DevOps CLI would try to automatically detect the organization, project and repository.

If you want to run any command for a particular orgainzation/project, you can explicity give it as an argument:
```
az boards work-item show --id 1 --organization https://dev.azure.com/MY-ORGANIZATION-NAME/
```
