<!-- GITHUB ANALYTICS -->

<h2 align="left">
  <img
    src="https://readme-typing-svg.demolab.com?font=Cormorant+Garamond&weight=600&size=30&duration=4000&pause=100000&color=C8A96B&vCenter=true&width=520&height=45&lines=GitHub+Analytics"
  />
</h2>

<p align="left">
These charts reflect my coding activity, contribution patterns, language usage, and engineering consistency across personal and collaborative projects.
</p>

<br/>

<!-- STATS -->

<p align="center">

<img
  height="170"
  src="https://github-readme-stats.vercel.app/api?username=huytran2005&show_icons=true&theme=transparent&hide_border=true&title_color=C8A96B&text_color=E5E7EB&icon_color=C8A96B"
/>

<img
  height="170"
  src="https://github-readme-stats.vercel.app/api/top-langs/?username=huytran2005&layout=compact&theme=transparent&hide_border=true&title_color=C8A96B&text_color=E5E7EB"
/>

</p>

<br/>

<!-- STREAK -->

<p align="center">

<img
  src="https://streak-stats.demolab.com?user=huytran2005&theme=transparent&hide_border=true&ring=C8A96B&fire=C8A96B&currStreakLabel=C8A96B&sideLabels=E5E7EB&dates=94A3B8"
/>

</p>

<br/>

<!-- CONTRIBUTION -->

<h3 align="left">
  <img src="https://readme-typing-svg.demolab.com?font=Cormorant+Garamond&weight=600&size=24&duration=4000&pause=100000&color=C8A96B&vCenter=true&width=300&height=35&lines=Contribution+Activity" alt="Contribution Activity" />
</h3>

<p align="center">

<img
  width="100%"
  src="https://raw.githubusercontent.com/huytran2005/huytran2005/output/github-contribution-grid-snake-dark.svg"
/>

</p>

<br/>

<p align="left">
  <img
    src="https://capsule-render.vercel.app/api?type=rect&color=0:C8A96B,100:0D1117&height=2&section=header"
  />
</p>

<!-- SNAKE WORKFLOW -->

<!--
Tạo file:
.github/workflows/snake.yml

Paste code dưới đây:
-->

```yaml
name: Generate Snake

on:
  schedule:
    - cron: "0 */12 * * *"

  workflow_dispatch:

jobs:
  build:
    runs-on: ubuntu-latest

    steps:
      - uses: Platane/snk@v3
        with:
          github_user_name: huytran2005
          outputs: |
            dist/github-contribution-grid-snake-dark.svg?palette=github-dark

      - uses: crazy-max/ghaction-github-pages@v4
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```