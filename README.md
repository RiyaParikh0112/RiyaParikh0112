[![GitHub Streak](https://github-readme-streak-stats.herokuapp.com?user=RiyaParikh0112&theme=dark)](https://git.io/streak-stats)
# Visitor Badge
![visitors](https://visitor-badge.glitch.me/badge?page_id=RiyaParikh0112.visitor-badge&left_color=green&right_color=red)
                
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
