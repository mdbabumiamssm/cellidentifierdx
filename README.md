1. **Project Name**: The name of your project.
2. **Description**: A brief description of what your project does.
3. **Installation**: Instructions for how to install your project.
4. **Usage**: Instructions for how to use your project after it's installed.
5. **License**: The license your project is distributed under.
6. Note: This software package is yet to be published (unpublished)! If you have used it for publication purpose, please share authorship with MD. BABU MIA, PHD; ICAHN SCHOOL OF MEDICINE AT MOUNT SINAI. Contact for detials: md.babu.mia@mssm.edu
# CellIdentifierDX

CellIdentifierDX is a Python package for identifying cell types using Bayesian scoring.

## Installation

You can install CellIdentifierDX using pip:

```bash
pip install cellidentifierdx
```

## Usage

Here's a basic example of how to use CellIdentifierDX:

```python
from cellidentifierdx import annotate_cell_types

reference_file = "/path/to/your/reference_file.xlsx"
expr_file = "/path/to/your/expr_file.csv"
tissue, cell_type_annotations = annotate_cell_types(reference_file, expr_file, 'sheetname')

for cluster_idx, cell_type, avg_score in cell_type_annotations:
    print(f"Cluster {cluster_idx} is annotated as {cell_type} with average Bayesian score of {avg_score}.")

```

## License

MIT
```
