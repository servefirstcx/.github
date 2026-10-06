# servefirstcx/.github

Organization-wide defaults for servefirstcx repositories.

## Pull request template

[`pull_request_template.md`](pull_request_template.md) pre-fills the description of every new pull request opened in GitHub's web interface, in any servefirstcx repository that doesn't have its own template.

The first line matters most: put the Jira ticket(s) the PR finishes after `Closes`, for example `Closes SF-1234` or `Closes SF-1234, SF-1235`. That links the PR to the ticket, so the ticket moves to Dev Complete when the PR merges and to Done (In Production) when its release reaches production. A ticket number in the branch name (`SF-1234-short-name`) does the same.

Pull requests created from the command line or by automation (`gh pr create --body …`, the API, AI agents) don't get the template, so include the `Closes SF-…` line yourself.

To change the template for a single repository, add its own `.github/pull_request_template.md`; it replaces this one there.

This repository must stay public for GitHub to apply these defaults. Keep anything internal out of it.
