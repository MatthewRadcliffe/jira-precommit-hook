jira-precommit-hook
-------------------

Goals:

- Distributable via npm (This will eventually be pushed to a public github repo)
- Testable
- Commit hook script contains the bare bones needed to call into this library.
  We may want to investigate use of existing
  [pre-commit](https://www.npmjs.com/package/pre-commit) module.


# NOTICE

Currently only configured for read-only access to JIRA.

# Project Configuration

**DESCRIPTION**
In order to communicate with your JIRA server, a .jirarc file needs to be placed in the root of the repo.

```json
{
	"projectName": "<Name of JIRA project - REQUIRED>",
	"host":"<URL location of JIRA project - REQUIRED>",
	"protocol":"[default:http|https]",
	"port": 80,
	"version": default:2,
	"verbose": false,
	"strictSSL": true
}
```
