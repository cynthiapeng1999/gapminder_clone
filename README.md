# Practice Project One: 200 Countries, 200 Years, 4 Minutes

## Introduction

This project, "200 Countries, 200 Years, 4 Minutes," recreates the renowned data visualization [Hans Rosling's 200 Countries, 200 Years, 4 Minutes](https://youtu.be/jbkSRLYSojo?si=5WkjOoiU_IPuKGsR). I used `pandas` and `sqlite3` to build the database, `matplotlib` for proof of concept, and finally `plotly.express` to produce the finished product.

## How to Reproduce

- Install [Miniconda](https://docs.anaconda.com/miniconda)
- Build the environment based on `environment.yml`

```bash
conda env create -f environment.yml
```

- Place the four CSV files from the `data/` folder into a `data/` folder in your working directory.
- Activate the environment and run `python create_gapminder_db.py` to create `gapminder.db` in the `data/` folder.
- Activate the environment and run  `python plot_with_px.py` to generate `gapminder_clone.html`