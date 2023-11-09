# trackintel-tutorial
Tutorial materials for trackintel library

## SIGSPATIAL 23 ReproTrack workshop

    

### Download Geolife 
- Download the Geolife GPS tracking dataset from [here](https://www.microsoft.com/en-us/download/details.aspx?id=52367). Unzip and copy the `Data` folder into `Data/geolife/`. The file structure should look like `Data/geolife/Data/000/...`.
- Create file `paths.json`, and define your working directories by writing:

```json
{
    "data_dir": "./Data/geolife/"
}
```