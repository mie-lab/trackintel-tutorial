# trackintel-tutorial
Tutorial materials for trackintel library

## SIGSPATIAL 23 ReproTrack workshop

Materials for the [1st ACM SIGSPATIAL International Workshop on Reproducibility in tracking data analysis and mobility research](https://mie-lab.github.io/reprotrack/)

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
    "data_dir": "./Data/geolife/"
}
```
