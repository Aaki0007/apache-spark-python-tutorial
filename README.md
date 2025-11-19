# Apache Spark with Python (PySpark) Tutorial

This repository contains the materials for a short **Apache Spark** tutorial session.

- Slides: see [`slides/`](./slides/) folder  
- Notebooks: see [`notebooks/`](./notebooks/) folder 

  - `pyspark_short_tutorial.ipynb` 

---

## 📑 Session Outline

This tutorial teaches you how to use Apache Spark for distributed data processing. By the end of this session, you will be able to:

1. **Understand Apache Spark** - What it is, when to use it, and why it's better than Pandas for large datasets
2. **Start a SparkSession** - Configure and launch Spark in local mode on your laptop
3. **Work with DataFrames** - Create, inspect, and transform data using Spark DataFrames
4. **Perform aggregations** - Use `groupBy` and aggregate functions to summarize data
5. **Query with Spark SQL** - Write SQL queries on DataFrames using familiar SQL syntax
6. **Join datasets** - Combine multiple tables using join operations
7. **Build ETL pipelines** - Extract, Transform, and Load data in a scalable way
8. **Read and write files** - Work with CSV and Parquet file formats

### What You'll Learn

- **When to use Spark vs Pandas**: Understanding the tradeoffs between single-machine and distributed computing
- **Lazy evaluation**: How Spark optimizes query execution by planning before executing
- **Working with large datasets**: Best practices for `.show()`, `.limit()`, and avoiding `.collect()` on big data
- **Spark SQL**: Leveraging your SQL knowledge to query distributed datasets
- **Real-world ETL patterns**: Building data transformation pipelines that can scale from your laptop to a cluster


---
## 🚀 Environment Setup

Before starting, please **fork this repository** and create a fresh Python virtual environment.  
All required libraries are listed in `requirements.txt`.

> ⚠️ If you encounter errors during `pip install`, try removing the version pinning for the failing package(s) in `requirements.txt`.  
> On Apple M1/M2 systems you may also need to install additional system packages (the “M1 shizzle”).

---

### macOS / Linux (bash/zsh)

```bash
# Select Python version (if using pyenv)
pyenv local 3.11.3

# Create and activate virtual environment
python -m venv .venv
source .venv/bin/activate

# Upgrade pip and install dependencies
pip install --upgrade pip
pip install -r requirements.txt
```

### Windows (PowerShell)
```bash
# Select Python version (if using pyenv)
pyenv local 3.11.3

# Create and activate virtual environment
python -m venv .venv
.venv\Scripts\Activate.ps1

# Upgrade pip and install dependencies
python -m pip install --upgrade pip
pip install -r requirements.txt
```

### Windows (Git Bash)
```bash
# Select Python version (if using pyenv)
pyenv local 3.11.3

# Create and activate virtual environment
python -m venv .venv
source .venv/Scripts/activate

# Upgrade pip and install dependencies
python -m pip install --upgrade pip
pip install -r requirements.txt
```

You’re now ready to run the session notebooks!

Deactivate the environment when you’re done:
```bash
deactivate
```
