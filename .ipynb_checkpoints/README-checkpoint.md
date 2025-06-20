# H2-GAE
Hierarchical & Heterogeneous Graph Autoencoder (H2-GAE)

```
.
├── configs
│   ├── data.yaml
│   ├── model.yaml
│   └── training.yaml
├── data
│   ├── processed
│   └── raw
│       ├── census
│       └── osm
│           
├── LICENSE
├── notebooks
├── pyproject.toml
├── README.md
└── src
    ├── data
    │   ├── __init__.py
    │   ├── census_loader.py
    │   ├── graph_builder.py
    │   └── osm_processor.py
    ├── evaluate
    │   ├── __init__.py
    │   └── sustainability_merics.py
    ├── models
    │   ├── __init__.py
    │   ├── H2-GAE.py
    │   ├── layers
    │   │   ├── hetero_gat.py
    │   │   └── hetero_pool.py
    │   └── losses.py
    ├── train
    │   ├── __init__.py
    │   ├── callbacks.py
    │   └── train.py
    └── utils
        └── seed.py

```


```
uv sync --dev
uv run ipython kernel install --user --env VIRTUAL_ENV $(pwd)/.venv --name=project
```