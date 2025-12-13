# PoliticheForestaliAmbientali.github.io

This repository hosts the website for Politiche Forestali Ambientali, automatically built from a Google Sheets spreadsheet using the Sheets2Website tool.

## How it works

1. **Source data**: The site content comes from a [Google Sheets spreadsheet](https://docs.google.com/spreadsheets/d/1pSLbsjGTy2WlU2rEn2NZCnbU7dqk7Kwj8G7AGNYGf8I/edit?usp=sharing).

2. **Configuration**: The `config.json` file specifies the URL of the Google Sheets to use.

3. **Automatic build**: A GitHub Actions workflow (`.github/workflows/sync-build-deploy.yml`) runs:
   - Automatically every day at 6:00 UTC
   - Manually when triggered

4. **Deployment**: The site is built and deployed to GitHub Pages.

## Content changes

To modify the site content:
1. Edit the data in the [Google Sheets spreadsheet](https://docs.google.com/spreadsheets/d/1pSLbsjGTy2WlU2rEn2NZCnbU7dqk7Kwj8G7AGNYGf8I/edit?usp=sharing)
2. The site will update automatically within 24 hours, or manually trigger the GitHub Actions workflow

## Repository structure

- `config.json`: Configuration with the Google Sheets URL
- `.github/workflows/sync-build-deploy.yml`: Workflow for automatic build and deployment