#update

Deploy a new version of the Lambda function using project files, update any associated web APIs

## Usage

```bash
claudia update {OPTIONS}
```

## Options

*  `--version`:  _optional_ A version alias to automatically assign to the new deployment
  * _For example_: development
*  `--source`:  _optional_ Directory with project files
  * _Defaults to_: current directory
*  `--config`:  _optional_ Config file containing the resource names
  * _Defaults to_: claudia.json
*  `--no-optional-dependencies`:  _optional_ Do not upload optional dependencies to Lambda.
*  `--use-local-dependencies`:  _optional_ Do not install dependencies, use local node_modules directory instead
*  `--cache-api-config`:  _optional_ Name of the stage variable for storing the current API configuration signature.
  If set, it will also be used to check if the previously deployed configuration can be re-used and speed up deployment
