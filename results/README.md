# Results

## `category_sales.csv`

This file contains the aggregated sales results for the synthetic dataset in `data/sales_dataset.csv.gz`.

The aggregation follows the notebook's analysis:

- Keep rows where `quantity > 5`.
- Group the remaining rows by `category`.
- Sum `quantity` into `total_quantity` and `total` into `total_sales`.

The CSV columns are `category`, `total_quantity`, and `total_sales`. Values were generated from the saved dataset and may differ from outputs previously recorded in the notebook.
