# AGILE Reproducibility Reviews 2024

## About

This repository contains code used for the organisation and management of the reproducibility review at AGILE 2024.
Read more about the review process and the reproducibility committee here: <https://reproducible-agile.github.io/2024/>.

The reproducibility reviews are published on OSF: <https://osf.io/qvr4s/>

[![Reproducible AGILE badge](https://raw.githubusercontent.com/reproducible-agile/reproducible-agile.github.io/master/public/images/badge/AGILE-reproducible-badge_square.png)](https://reproducible-agile.github.io/)

## Contents/Usage

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/reproducible-agile/reviews-2023/HEAD)

To work on the main R Markdown file, `agile-reproducibility-reviews.Rmd`, which includes _all_ information and documentation of the reproducibility review, run (requires GNU Make, and `virtualenv` for Python)

### 1. Start the container with AGILE Reproducibility Reviews Customization

```bash
make
```
The `Makefile`'s default target will create a virtual Python environment to execute [`repo2docker`](https://repo2docker.readthedocs.io/) using the files in this repository, notably `install.R` where you must add required R packages, and the `Dockerfile` where all system dependencies and remaining software is installed and configured.

### 2. Start RStudio

Then open the Jupyter UI at the link shown in the console.
In the UI, go to "New" > "RStudio" to get an integrated development environment with the required dependencies.

### 3. Prepare your report 

You can copy and paste [report-template/reproreview-template.Rmd](report-template/reproreview-template.Rmd)

```bash
cp report-template/reproreview-template.Rmd reports/[my_report].Rmd
```

### 4. Build your PDF

On RStudio, click `knit` or tick the `Knit on save` button.


## License

Copyright 2024 Daniel Nüst, published under The Apache License, Version 2.0.
