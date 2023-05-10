name: Deploy to GitHub Pages

on:
  # Automatic build on push, choose the branch you want to use here
  push:
    branches: "master"
  # If you want to be able to build it manually from any branch
  workflow_dispatch:

jobs:
  deploy:
    runs-on: ubuntu-latest
    steps:
      - uses: ivancea/mac-renderer@v1
        with:
          github-token: ${{ secrets.GITHUB_TOKEN }}

# Minimum required permissions
permissions:
  contents: read
  pages: write
  id-token: write