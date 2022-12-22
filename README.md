# aws-open-data

[![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/giswqs/aws-open-data/blob/master/aws_open_datasets.ipynb)
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/giswqs/aws-open-data/HEAD?labpath=aws_open_datasets.ipynb)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Introduction

The [AWS Open Data](https://registry.opendata.aws/) program hosts a lot of publicly available datasets. This repo compiles the list of all datasets on AWS as a CSV file and as a JSON file, making it easier to find and use them programmatically. The list is updated daily.

A complete list of AWS open datasets as individual YAML files is available [here](https://github.com/awslabs/open-data-registry).

## Usage

This repo provides the list of AWS open datasets in two formats:

- Tab separated values (TSV) file: [aws_open_datasets.tsv](https://github.com/giswqs/aws-open-data/blob/master/aws_open_datasets.tsv)
- JSON file: [aws_open_datasets.json](https://github.com/giswqs/aws-open-data/blob/master/aws_open_datasets.json)

The TSV file can be easily read into a Pandas DataFrame using the following code:

```python
import pandas as pd

url = 'https://github.com/giswqs/aws-open-data/raw/master/aws_open_datasets.tsv'
df = pd.read_csv(url, sep='\t')
df.head()
```

## Related Projects

- A list of open datasets on AWS: [aws-open-data](https://github.com/giswqs/aws-open-data)
- A list of open geospatial datasets on AWS: [aws-open-data-geo](https://github.com/giswqs/aws-open-data-geo)
- A list of open geospatial datasets on AWS with a STAC endpoint: [aws-open-data-stac](https://github.com/giswqs/aws-open-data-stac)
- A list of STAC endpoints from stacindex.org: [stac-index-catalogs](https://github.com/giswqs/stac-index-catalogs)
- A list of geospatial datasets on Microsoft Planetary Computer: [Planetary-Computer-Catalog](https://github.com/giswqs/Planetary-Computer-Catalog)
- A list of geospatial datasets on Google Earth Engine: [Earth-Engine-Catalog](https://github.com/giswqs/Earth-Engine-Catalog)