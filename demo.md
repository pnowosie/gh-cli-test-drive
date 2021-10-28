# GH tool demo - for Golem!

## Abstract

- switching context harms productivity
- switching windows (to internet browser) may harm it as well
- let's use `gh` to never need to switch away from the terminal (vim)


## `gh` is fun to play / discover

- Demo!


## JIRA <-> GitHub integration
(current version)

- when PR is drafted -> ticked moves to `IN PROGRESS`
- when PR is merged -> ticket changes to `DONE`
- :( no way to change status to `IN REVIEW`

👉 We should open PRs as soon as posible!
...but how, when no real work has been done?
...and there is no branch to commit?


## Let's open a PR (really quick)

- whats-on-me

```bash
masta
g p
g o -b pnowosie/dev-standup-demo-APPS-324

echo "TITLE PLEASE\n\n" > /tmp/quick-pr.tpl
whats-on-me 324 >> /tmp/quick-pr.tpl
cat .github/pull_request_template.md >> /tmp/quick-pr.tpl
g commit --allow-empty -t /tmp/quick-pr.tpl

```
