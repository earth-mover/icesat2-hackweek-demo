# ICESat-2 Hackweek Demo

This repository contains demonstration notebooks showcasing the Earthmover Platform for accessing and analyzing large-scale climate and ice sheet datasets. The demos illustrate how to use Arraylake and Icechunk to work with petabyte-scale geoscience data directly from cloud storage.

## Overview of the Earthmover Platform

The Earthmover Platform provides seamless access to large-scale Earth observation datasets through:
- **Arraylake**: A cloud-native data platform for scientific datasets
- **Icechunk**: A version-controlled, cloud-optimized data format built on Zarr
- **Direct cloud access**: Query datasets without downloading, using familiar Python tools like Xarray

## Notebooks

### Notebook 1: ERA5 Climate Analysis (`01-era5-analysis.ipynb`)
Demonstrates working with ERA5 weather reanalysis data:
- Discover and access datasets via Arraylake Client
- Use Icechunk and Xarray for efficient cloud-based data access
- Explore Icechunk's version history and branching capabilities
- Perform spatial and temporal analysis on the ERA5 dataset
- Create custom data subsets and write to new Icechunk repositories

### Notebook 2: ICESat-2 ATL15 Land Ice Height Change (`02-icesat2-atl15.ipynb`)
Combines ICESat-2 ATL15 ice sheet data with ERA5 climate data:
- Access ATL15 dataset through Arraylake's hierarchical data structure
- Work with different spatial resolutions using Zarr groups
- Reproject climate data to match ice sheet grids
- Analyze correlations between temperature and ice sheet height changes
- Demonstrate multi-dataset analysis workflows

## Getting Started

### 1. Install the Arraylake Client
```bash
pip install arraylake icechunk
```

### 2. Navigate to the Arraylake Web App
Visit [https://app.earthmover.io](https://app.earthmover.io) to explore available datasets

### 3. Clone the Demo Repository
```bash
git clone https://github.com/earth-mover/icesat2-hackweek-demo.git
```

### 4. Authentication
Run the notebooks and authenticate when prompted using your hackweek email address or Google account. The authentication uses OAuth2 and will open a browser window for login.

## License

This project is released under the [MIT License](LICENSE).
