# Falco Rules GitHub Actions Workflow

This repository contains a GitHub Actions workflow to validate Falco security rules. The workflow is defined in `falco.yml`.

## How It Works
- Runs on `push` and `pull_request` events.
- Uses a Docker container to validate Falco rules.
- Outputs validation results in GitHub Actions logs.

## Usage
1. Modify Falco rules.
2. Push changes or create a pull request.
3. The workflow will validate the rules automatically.
4. Check logs for validation results.
