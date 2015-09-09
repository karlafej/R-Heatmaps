# Generating Heatmaps in R Workshop

This is the Github repository for the event - https://github.com/minisciencegirl/studyGroup/issues/47. The official event details are as follows:

* Date: September 8, 2015
* Time: 5:30pm
* Room: BCCA (Dorothy Lam Room)

# Preparation for the Workshop

The workshop will contain coding exercises where you can run R code to generate some heatmaps. If you are interested in doing this, please bring your laptop to the workshop and do the following preparation steps.

1. [git](https://git-scm.com/) clone this repository:

    ```
    git clone git@github.com:tinyheero/R-Heatmaps.git
    ```
    
    The repository comes with the following files/folders:
    
    * [Generating-Heatmaps-in-R.pdf](https://github.com/tinyheero/R-Heatmaps/blob/master/Generating-Heatmaps-in-R.pdf): This is the slidedeck for the workshop.
    * heatmap-cluster.Rmd: This is an Rmarkdown file that contains a tutorial and code on how to generate the images shown in the slide deck.
    * [heatmap-cluster.html](http://htmlpreview.github.io/?https://github.com/tinyheero/R-Heatmaps/blob/master/heatmap-cluster.html): The final output of `heatmap-cluster.Rmd`.
    * data: Folder containing the data files required for the `heatmap-cluster.Rmd` file.

    If you are unable to `git clone` this repository, you can also download a packaged version of this repository through the [releases link (at the top)](https://github.com/tinyheero/R-Heatmaps/releases). Please contact me if you are having trouble with either step.

2. Install [Rstudio](https://www.rstudio.com/) (if you haven't already). The code was tested to work with RStudio 0.99.484.
3. Inside of Rstudio, make sure you install the following R packages (the version numbers of each package have been provided to indicate what they were tested on to work with)

    * [dplyr](https://cran.r-project.org/web/packages/dplyr/index.html) (v0.4.3)
    * [knitr](https://cran.r-project.org/web/packages/knitr/index.html) (v1.11)
    * [d3heatmap](https://cran.r-project.org/web/packages/d3heatmap/index.html) (v0.6.1)
    * [RColorBrewer](https://cran.r-project.org/web/packages/RColorBrewer/index.html) (v1.1-2)
    * [reshape2](https://cran.r-project.org/web/packages/reshape2/index.html) (v1.4.1)
    * [ggplot2](https://cran.r-project.org/web/packages/ggplot2/index.html) (v1.0.1)

    Packages can be installed using the `install.packages` function. For example:

    ```
    install.packages("dplyr")
    ```

4. Make sure you can render the `heatmap-cluster.Rmd` file by opening the `heatmap-cluster.Rmd` file in RStudio and then pressing the "Knit HTML" button. If it works, then you should see a separate open window open with a document titled "Generating Heatmaps in R".

# FAQ

1. Why can't I load the `mat.lim` variable?

    This is likely occurring because the `data/mirna-normalized-expression-subset-lim-2015.txt` file is missing or R can't find the file. If you are using the RStudio to open the `heatmap-cluster.Rmd`, you need to make sure that the working directory of your R contains both the `heatmap-cluster.Rmd` and `data/mirna-normalized-expression-subset-lim-2015.txt`. Specifically, the text file needs to be in a `data` folder. 
    
    The best procedure is `git clone` the repository or download the release package, open `heatmap-cluster.Rmd` in RStudio, then at the top go `Session -> Set Working Directory -> To Source File Location`. 

# Contact

Feel free to contact me for help regarding the content in this workshop:

* email: fongchunchan@gmail.com
* twitter: [https://twitter.com/fongchunchan](https://twitter.com/fongchunchan)
* blog: [http://tinyheero.github.io/](http://tinyheero.github.io/)
