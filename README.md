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

## Key Takeaways
- Multi-table database design with SQL views: Loaded four separate tables into SQLite and used `CREATE VIEW` to join them, keeping raw data clean and the plotting script simple.
- Encoding multiple variables in a single chart: The bubble chart maps five dimensions simultaneously (x, y, size, color, animation). Choices like a log scale for GDP required thinking about both the data distribution and the audience.
- Interactive vs. static output: Chose `plotly.express` over `matplotlib` to produce an interactive HTML file — letting viewers explore countries and years themselves. Knowing when each tool is appropriate matters as much as knowing how to use them.
