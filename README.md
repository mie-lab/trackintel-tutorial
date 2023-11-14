# trackintel-tutorial
Tutorial materials for trackintel library

## SIGSPATIAL 23 ReproTrack workshop

We organized the  [1st ACM SIGSPATIAL International Workshop on Reproducibility in tracking data analysis and mobility research](https://mie-lab.github.io/reprotrack/), featuring a keynote talk by Prof. Edzer Pebesma a tutorial and a hands-on session. 

* Keynote by Edzer Pebesma: Slides: [here](https://docs.google.com/presentation/d/1M2SB1ibV0Jzt9FZFmdrEp_xWIZdZLC2X89xJdWaTSZs/edit?usp=sharing)\\ Abstract: In this talk I will discuss of reproducibility in general, why it
matters for good science, the differences to replicability, and the
challenges aspects to reproducing scientific computations.  I will
also discuss the practice of how we conduct science, how and why we
write, submit and review research papers, how and why we write, share
and publish research software, and the connection between these two.
Although not an expert in the area of tracking data analysis, I will
try to shed some light on particular challenges for reproducibility
of tracking data analysis, and try to formulate some recommendations.
* Introduction [slides](sigspatial23/workshop_slides.pdf)
* [Tutorial](sigspatial23/Introduction_to_trackintel.ipynb) how to use the Trackintel library
* Hands-on session with several tasks in the [sigspatial23](sigspatial23) folder


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
