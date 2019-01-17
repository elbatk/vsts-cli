# Output formats for Azure DevOps CLI commands

The output formats are inherited from the Azure CLI. You can set the default output format value by running following command.
```
az configure
```
You can find information about output formats [here](https://docs.microsoft.com/en-us/cli/azure/format-output-azure-cli?view=azure-cli-latest).

The Azure CLI uses JSON as its default output option, but offers various ways for you to format the output of any command.  Use the `--output` (or `--out` or `-o`) parameter to format the output of the command into one of the output types noted in the following table. 

--output | Description
---------|-------------------------------
`json`   | JSON string. `json` is the default.
`jsonc`  | Colorized JSON string.
`table`  | Table with column headings.
`tsv`    | Tab-separated values.
`yaml`   | YAML, a machine-readable alternative to JSON.
