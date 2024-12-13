## Building a Data Analysis pipeline using a shell script tutorial
adapted from [Software Carpentry](http://software-carpentry.org/)

This example data analysis project analyzes the word count for all words in 4
novels. It reports the top 10 most occurring words in each book in a [report](doc/count_report.qmd).

### Current usage:

#### Set-up (first time only)

1. Clone this repo, and using the command line, navigate to the root of this project.

2. Run the following commands to create the conda environment:

```
conda-lock install --name da-pipeline-sh conda-lock.yml
```

#### Run the analysis 

Activate the conda environment:

```
conda activate da-pipeline-sh
```

Run the anaysis and generate the report using bash:

```
bash runall.sh
``````

Run the anaysis and generate the report using make:

```
make all
``````

clean generated files to run again:

```
make clean
``````
### Depenedencies
- Quarto
- Python & Python libraries:
    - `click`
    - `matplotlib`
    - `pandas`
