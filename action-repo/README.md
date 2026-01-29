# Action Repo
This repository is used to generate GitHub events.
It is a dummy repo where you can make commits, create pull requests, and merge branches.
## Webhook
- A webhook is configured to send events (push, pull_request, and merge via PR) to the Flask server in the webhook-repo.
### How to Test
1. Make a commit → triggers push event.
2. Open a pull request → triggers pull_request event.
3. Merge a pull request → triggers merge event.
These events will be received by the webhook-repo and displayed in the UI.
