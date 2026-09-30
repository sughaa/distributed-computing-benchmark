# Distributed Computing Benchmark

A small benchmark comparing data processing with Pandas and PySpark. The notebook creates a synthetic sales dataset, filters rows where `quantity > 5`, groups by `category`, and compares the aggregated results and execution times.

## Project structure

```text
.
├── Benchmark_datasets.ipynb       # Pandas and PySpark benchmark
├── data/
│   └── sales_dataset.csv.gz        # One million synthetic sales records
└── results/
    ├── category_sales.csv          # Aggregated sales by category
    └── README.md                   # Result file details
```

The CSV files in `data/` and `results/` were generated separately from the notebook's in-memory sample. They use the same schema and aggregation logic, but their values can differ from the notebook's saved outputs.

## Requirements

- Python 3
- Jupyter Notebook or JupyterLab
- pandas
- numpy
- pyspark
- matplotlib

Install the Python packages with:

```bash
python -m pip install pandas numpy pyspark matplotlib jupyter
```

## Run the benchmark

Start Jupyter from the project directory, open `Benchmark_datasets.ipynb`, and run the cells in order. The notebook builds its own one-million-row dataset in memory and reports the Pandas and PySpark timings. Results can vary by machine and runtime environment.
