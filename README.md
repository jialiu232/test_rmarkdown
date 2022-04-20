# Visualize output file generated from Rmarkdown on Github 

**Purpose**:

`*.rmd` generated html files cannot be shown on github. I want to figure out why and how to nicely show the `*.rmd` files in a readable format on github.

**Reason**:

It turns out that github cannot render `.rmd` files.

**One of the solutions**:

1. change `output: html_document` to `output: github_document` in `title.rmd` file;
2. knit the `title.rmd` file in Rstudio will produce a `title.md` file, and a `title_files/` folder if any plots are generated;
3. then stage and push the `title.md` file as well as the `title_files/` if there is one to github


Since Github can render the `.md` files, now you should now be able to read `title.md` on github. 

Reference: https://gist.github.com/JoshuaTPierce/b919168421b40e06481080eb53c3fb2f
