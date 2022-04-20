# Visualize output file rendered from Rmarkdown on Github 

**Purpose**:

Suppose you created a github repo, you cloned it to your local computer, worked on a Rmarkdown file and rendered it to generate an `html` file, and finally you updated all these changes to your github. However, neither the `*.rmd` nor the `*.rmd` generated `html` files can be displayed nicely in a reader friendly way in your github repo. Here I want to figure out why that's the case and how to nicely show the `*.rmd` output files in a readable format on github.

**Reason**:

It turns out that github cannot render `.rmd` files.

**A 3-step solution**:

Suppose your file name is `title.rmd`,

1. change `output: html_document` to `output: github_document` in `title.rmd` file;
2. knit the `title.rmd` file in Rstudio will produce a `title.md` file, and a `title_files/` folder if any plots are generated;
3. then stage, commit and push the `title.md` file as well as the `title_files/` (if there is one) to your github repo (Feel free to update any other changes to github as needed).


Since Github can render `.md` files, now just click the `title.md` in your github repo and you should be able to see what you want. 

Reference: 
- https://gist.github.com/JoshuaTPierce/b919168421b40e06481080eb53c3fb2f
- https://yihui.org/en/2018/10/rmd-github/
