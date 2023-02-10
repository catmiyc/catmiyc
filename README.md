- 👋 Hi, I’m @catmiyc
- 🤓 I’m learning Front-End Development

<!---
catmiyc/catmiyc is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->


[![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=catmiyc)](https://github.com/anuraghazra/github-readme-stats)

[![GitHub Streak](https://streak-stats.demolab.com/?user=catmiyc)](https://git.io/streak-stats)

name: Waka Readme

on:
  schedule:
    # Runs at 12am IST
    - cron: '30 18 * * *'
  workflow_dispatch:
jobs:
  update-readme:
    name: Update Readme with Metrics
    runs-on: ubuntu-latest
    steps:
      - uses: anmol098/waka-readme-stats@master
        with:
          WAKATIME_API_KEY: ${{ secrets.WAKATIME_API_KEY }}
          GH_TOKEN: ${{ secrets.GH_TOKEN }}
