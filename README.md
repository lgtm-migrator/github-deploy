# github-deploy
Python package that automates deployment of files to multiple repositories all at once


## Usage

#### Creating or Updating files on github

`github-deploy`

```shell script
github-deploy --org [org] --token [PAT_TOKEN] --dest [LOCATION TO UPLOAD FILE] --source [SOURCE FILE LOCATION]
```

Example:

```shell script
github-deploy --org tj-actions --token [PAT_TOKEN] --dest '.github/workflows/auto-approve.yml' --source auto-approve.yml
```

> NOTE: `auto-approve.yml` is located on your local system.


#### Deleting files on github

`github-delete`

```shell script
github-delete --org [org] --token [PAT_TOKEN] --dest [LOCATION TO DELETE]
```

Example:

```shell script
github-delete --org tj-actions --token [PAT_TOKEN] --dest '.github/auto-approve.yml'
```
