# Instructions

## Setting up the Virtual Environment

For Unix-like using virtualenv
```bash
sudo apt-get install virtualenv python
virtualenv -p /usr/bin/python3.6 venv
```
Using Anaconda/conda (i.e. Windows OS)
```shell
conda create --name data-meetup-env --path python=3.6 
```

## Install the Python Dependencies

For Unix-like using virtualenv
```bash
source venv/bin/active
pip install -r requirements.txt
```

Using Anaconda/conda (i.e. Windows OS, Mac OS)
```shell
# Activate the environment
# depending on which version of conda you have
conda activate data-meetup-env
# or
source activate data-meetup-env
# installing the packages
pip install -r requirements.txt
```


## Jupyter Notebook

Setting up the theme (not necessary!) like the talk
```bash
source venv/bin/active
jt -t chesterish -fs 12 -cellw 90% -nfs 12 -tfs 12 -fs 12 -m auto -T -N
```

Run the interactive Presentation
```bash
jupyter nbconvert Pandas-vs-Dask-rezbaz2019-slides.ipynb --to slides --post serve --SlidesExporter.reveal_scroll=True
```

## Links

### Similar presentations
[Hunter Analytics Meetup Feb 2019](https://github.com/newwwie/data-analytics-meetup/tree/master/talks/Feb2019-Intro-Pandas-Dask)

### Datasets

Example: Example-CSV-time-series
[Electrical consumption data](https://archive.ics.uci.edu/ml/machine-learning-databases/00235/household_power_consumption.zip)

Example: Example-Dask-multi-csvs
[NYC Flights data](https://storage.googleapis.com/dask-tutorial-data/nycflights.tar.gz)

Example: Example-Dask-bag
[Ask Ubuntu on Stack Exchange posts](https://archive.org/download/stackexchange/askubuntu.com.7z)


### Various

Bulding and interactive data presentation (aka Creating slides) with Jupyter Notebook
[Jupyter Presentation](https://medium.com/learning-machine-learning/present-your-data-science-projects-with-jupyter-slides-75f20735eb0f)

Reading how I build the Dask Bag example
[Dask example](https://sigdelta.com/blog/dask-introduction/) 

Dask Links

* [Dask Cluster Dashboard](http://docs.dask.org/en/latest/diagnostics-distributed.html)

* [Dask data pipeline template](http://docs.dask.org/en/latest/custom-graphs.html#example)