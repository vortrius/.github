#!/bin/bash

# Use token from environment variable
NPMRC_FILE=~/.npmrc
NPMRC_CONTENT="# Install vortrius packages from GitHub Packages Registry
@vortrius:registry=https://npm.pkg.github.com
//npm.pkg.github.com/:_authToken=${TOKEN}"

# Create or overwrite the .npmrc file
echo "$NPMRC_CONTENT" > "$NPMRC_FILE"
chmod 600 "$NPMRC_FILE"
echo "Successfully configured ~/.npmrc with your GitHub token."

# Usage
# curl -s https://example.com/npmrc-setup.sh | TOKEN=your_github_token bash
