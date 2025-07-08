# 📁 My GitHub Repository

![Top Language](https://img.shields.io/github/languages/top/janitha-visna/janitha-visna)
![Languages Count](https://img.shields.io/github/languages/count/janitha-visna/janitha-visna)

## 📊 Language Statistics

![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=janitha-visna&layout=compact)

## 🚀 About This Project

This repository showcases my work across various programming languages, mainly focusing on full-stack web development and scripting.

## 🛠 Technologies Used

- **JavaScript**
- **TypeScript**
- **PHP**

---

### 🔄 Automatic GitHub Metrics Updates

To keep your stats updated automatically, you can set up GitHub Actions:

Create a workflow file at `.github/workflows/metrics.yml`:

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
