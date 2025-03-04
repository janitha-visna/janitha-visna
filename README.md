# My GitHub Repository

![Repository Languages](https://img.shields.io/github/languages/top/janitha-visna/janitha-visna)
![Languages Count](https://img.shields.io/github/languages/count/janitha-visna/janitha-visna)

## 📊 GitHub Language Stats

![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=YOUR_GITHUB_USERNAME&layout=compact)

## 🚀 About This Project

This repository contains a project built using multiple programming languages. Below is an overview of the top languages used.

## 🛠 Technologies Used

- Programming Language 1
- Programming Language 2
- Programming Language 3

---

### 📌 How to Set Up GitHub Metrics for Automatic Updates

To keep your programming language stats updated in your `README.md`, you can use **GitHub Actions**.

#### 1️⃣ Create a GitHub Action for Metrics

1. Go to your repository.
2. Navigate to `Settings` → `Actions` → `New Workflow`.
3. Create a new workflow file: `.github/workflows/metrics.yml`
4. Add the following code:

```yml
name: Generate Metrics

on:
  schedule:
    - cron: "0 0 * * *" # Runs daily
  workflow_dispatch:

jobs:
  metrics:
    runs-on: ubuntu-latest
    steps:
      - name: Generate GitHub Metrics
        uses: lowlighter/metrics@latest
        with:
          filename: metrics.svg
          token: ${{ secrets.GITHUB_TOKEN }}
          base: languages
