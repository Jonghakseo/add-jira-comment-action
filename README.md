# Pull-Request Jira Task Comment

## github action file example (for use)

```yml
name: PR Comment Jira

on:
  pull_request:
    types: [ opened, synchronize ]

jobs:
  add-jira-task-comment:
    runs-on: ubuntu-latest
    steps:
      - uses: creatrip/jira-task-comment-action@v1
#        with:
#          prefix: 'comment prefix'
#          suffix: 'comment suffix'
#          regexp default '(proxy|lan|com|travel)(\\s|-)(\\d+)' 
#          regexp: 'override find task regexp'

```
