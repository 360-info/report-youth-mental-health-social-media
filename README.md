# Youth Mental Health & Social Media  
### [📊&nbsp;Get&nbsp;the&nbsp;chart](https://public.flourish.studio/story/2043228/)  [📊&nbsp;Get&nbsp;the&nbsp;data](data) • [💻&nbsp;Reproduce&nbsp;the&nbsp;analysis](#-reproduce-the-analysis)

A recent report published in August 2023 found “no evidence suggesting that the global penetration of social media is associated with widespread psychological harm”

This contradicts earlier reports that found the opposite, particularly in regards to Instagram’s negative effects on girls.

Demonstrating a direct correlation between social media use and psychological harm is difficult, but damage or benefit to specific classes of people seems to be easier.

This package has an element that explores Rural Australia as one of several case studies - we have a data visualisation expert providing data visualisations on this.

360info’s special report on Social Media and Youth Mental Health explores which groups are most often harmed or helped by social media use. With a focus on the Indo Pacific region, which has some of the deepest social media use in the world, the special report looks at the data to get to the bottom of this complicated story  

<div class="flourish-embed" data-src="story/2043228"><script src="https://public.flourish.studio/resources/embed.js"></script></div>

## ♻️ Use + Remix rights

![[Creative Commons Attribution 4.0](https://creativecommons.org/licenses/by/4.0)](https://mirrors.creativecommons.org/presskit/buttons/80x15/png/by.png)

These charts, as well as the analyses that underpin them, are available under a Creative Commons Attribution 4.0 licence. This includes commercial reuse and derivates.

<!-- Do any of the data sources fall under a different licence? If so, describe the licence and which parts of the data fall under it here! if most of it does, change the above and replace LICENCE.md too -->

Data in these charts comes from:

* https://www.abs.gov.au/census/find-census-data/datapacks?release=2021&product=GCP&geography=AU&header=S  
* https://www.abs.gov.au/census/find-census-data/geopackages?release=2021&geography=AUS&table=G19&gda=GDA2020  

**Please attribute 360info and the data sources when you use and remix these visualisations.**

## 💻 Reproduce the analysis

### Quickstart: use the dev container

This project comes with a ready-to-use [dev container](https://code.visualstudio.com/docs/remote/containers) that includes everything you need to reproduce the analysis (or do a similar one of your own!), including [R](https://r-project.org) and [Quarto](https://quarto.org).

1. [Launch this project in GitHub Codespaces](https://github.com/codespaces/new?hide_repo_select=true&ref=main&repo=[report_codespaces_id])
2. If you have Docker installed, you can build and run the container locally:
  - Download or clone the project
  - Open it in [Visual Studio Code](https://code.visualstudio.com)
  - Run the **Remote-Containers: Reopen in Container** command

Once the container has launched (it might take a few minutes to set up the first time), you can run the analysis scripts with:

```sh
quarto render
```

Or look for the `.qmd` files to modify the analysis.

### Manual setup

To setup a development environment manually, 

You'll need to:
- [Download and install Quarto](https://quarto.org/docs/get-started)
- [Download the install R](https://www.r-project.org)
- Satisfy the R package dependencies. In R:
  * Install the [`renv`](https://rstudio.github.io/renv) package with `install.packages("renv")`,
  * Then run `renv::restore()` to install the R package dependencies.
  * (For problems satisfying R package dependencies, refer to [Quarto's documentation on virtual environments](https://quarto.org/docs/projects/virtual-environments.html).)

Now, render the `.qmd` files to the `/out` directory with:

```sh
quarto render
```

## ❓ Help

If you find any problems with our analysis or charts, please feel free to [create an issue](https://github.com/360-info/[report repo name]/issues/new)!
