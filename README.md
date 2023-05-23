# NOMAD Workflows documentation
This repository contains all documentation regarding custom and automatic Workflow schemas in NOMAD. We will divide it in four differentiated resources (plus an extra optional **Introduction** section):
1. **Tutorials**: general tutorials to learn the basics of workflows in your specific field of expertise (experiments or simulations).
2. **How-tos**: very specific and task-oriented guides.
3. **References**: references and information of keywords used in the documentation.
4. **Explanations**: detailed descriptions of the different parts of Workflows in NOMAD.


### How to launch locally for debugging

In the workflow-documentation directory, create your own virtual environment with Python3.9:
```
python3 -m venv .pyenvdoc
```
and activate it in your shell:
```
. .pyenvdoc/bin/activate
```

Make sure you have the latest pip version:
```
pip install --upgrade pip
```

Pip-install `mkdocs` and `mkdocs-material`:
```
pip install mkdocs
pip install mkdocs-material
```

Launch locally:
```
mkdocs serve
```

The output on the terminal should have these lines:
```
...
INFO     -  Building documentation...
INFO     -  Cleaning site directory
INFO     -  Documentation built in 0.29 seconds
INFO     -  [14:31:29] Watching paths for changes: 'docs', 'mkdocs.yml'
INFO     -  [14:31:29] Serving on http://127.0.0.1:8000/
...
```
Then click on the http address to launch the MKDocs.