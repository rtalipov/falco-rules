# Release Falco Rulesfile Workflow  

## Overview  
This GitHub Actions workflow automates the validation and release of Falco custom rules. It ensures that the rules are correctly formatted and then publishes them as an OCI artifact to GitHub Packages.  

## Workflow Steps  
1. **Falco Rule Validation**  
   - Checks out the repository.  
   - Validates the Falco rules using the official Falco container.  

2. **Release Rulesfile** (Runs after validation)  
   - Checks out the Falcoctl repository and sets up Golang.  
   - Builds `falcoctl` from source.  
   - Checks out the rules repository.  
   - Uploads the validated rules file as an OCI artifact to GitHub Packages.  

## OCI Artifact Details  
- The rules file is stored in GitHub's container registry (`ghcr.io`).
