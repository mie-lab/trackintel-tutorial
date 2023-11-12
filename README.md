# trackintel-tutorial
Tutorial materials for trackintel library

## SIGSPATIAL 23 ReproTrack workshop

Materials for the [1st ACM SIGSPATIAL International Workshop on Reproducibility in tracking data analysis and mobility research](https://mie-lab.github.io/reprotrack/)

Try the trackintel tutorial online in a MyBinder notebook [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/mie-lab/trackintel-tutorial/HEAD?urlpath=https%3A%2F%2Fgithub.com%2Fmie-lab%2Ftrackintel-tutorial%2Fblob%2Fmain%2Fsigspatial23%2FIntroduction_to_trackintel.ipynb)
### Installing the dependencies
- Clone the trackintel-tutorial repository into a local folder
```shell
    cd your-desired-folder
    git clone https://github.com/mie-lab/trackintel-tutorial.git
    cd trackintel-tutorial
```
- Install the reprotrack environment from the provided environment.yml file (with conda)
```shell
    conda env create -f sigspatial23/environment.yml
    conda activate reprotrack
```
- Test the environment configuration
```shell
    python -c "import trackintel; print(trackintel.__version__)"
```

### Geolife sample data 
- The `Data/Geolife/Data` folder contains a subset of selected 20 users from the original [Geolife](https://www.microsoft.com/en-us/download/details.aspx?id=52367) GPS tracking dataset. 
- In the file `paths.json`, we have defined the data directories by writing:

```json
{
    "data_dir": "./Data/Geolife/Data"
}
```
