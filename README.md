# test_rmarkdown

Purpose of this test:

`.rmd` generated html files cannot be shown on github. I want to figure out how to nicely show the `.rmd` files in a readable format on github.

Potential solutions:

1. change "output:html_document" to "output:github_document" in `.rmd` files; knit the `.rmd` file in Rstudio will produce `.md`; and then only stage and push the `.md` file to github.
