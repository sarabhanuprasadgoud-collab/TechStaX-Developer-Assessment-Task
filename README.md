# Overview

This project is part of the Techstax Developer Assessment. It demonstrates integration between GitHub Actions, Webhooks, Flask, MongoDB, and a UI that polls for updates every 15 seconds.
The solution is split into two repositories:
- action-repo → A dummy repository to trigger GitHub events (push, pull_request, merge).
- webhook-repo → A Flask application that receives webhook events, stores them in MongoDB, and serves them to a minimal UI.
---
📂 Repository Structure
1. `action-repo`
- Purpose: Generate GitHub events (Push, Pull Request, Merge).
- Contains:
  	- Branches for testing (main, dev, staging).
	- Sample commits and PRs.
- Configured webhook:
  	- Points to the Flask endpoint in webhook-repo.
2. `webhook-repo`
- Purpose: Webhook receiver + MongoDB storage + UI.
- Contains:
  	- app.py → Flask server with /webhook and /events routes.
	- requirements.txt → Dependencies.
	- templates/index.html → Minimal UI polling script.
	- README.md → Setup instructions.
---
