# Github Actions - CI-Configs
A list of Github Actions worksflows for automating different tasks

## Github Actions Basic Workflow
A sample yaml config. For better understanding [read the official documentation on how to get started](https://docs.github.com/en/actions/learn-github-actions/workflow-syntax-for-github-actions)

```yaml
name: Github Actions

# Trigger that will start the workflow
on:
  push:
  workflow_dispatch:
# or (read https://docs.github.com/en/actions/learn-github-actions/events-that-trigger-workflows)
#on: [pull_request, issues]

# declare jobs
jobs:
  my-job:
    name: My Job
    runs-on: ubuntu-latest
    steps:
    - name: Print a greeting
      run: |
        echo Hello there!
```

## Categories

### Compiling - C
These workflows compile stuff.

### Scraping - S
These workflows scrape stuff from the web into files / dbs.

### Delivery - D
These workflows deliver files (upload, release, send)

### API Tasks - A
These workflows use APIs to do tasks

### Updaters - U
These workflows update stuff

### Testers - T
These workflows are for testing all stuff

### Notifyers - N
These workflows are only for notifying


## How to use
Copy the workflow file into `.github/workflows/workflow_name.yml` and push to Github. If you're using Keys to push to Github make sure it has `Actions` permission or the push will be rejected.


## List
