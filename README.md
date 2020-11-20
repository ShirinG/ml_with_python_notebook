# Modifying pretrained nets - transfer learning

## Data

- download from

https://www.kaggle.com/moltean/fruits

- and save to working directory of this repo

## pull Dockerimage

```bash
docker pull tensorflow/tensorflow 
```

## start Jupyterlab

Run a Jupyter notebook server with your own notebook directory (assumed here to be ~/notebooks). To use it, navigate to localhost:8888 in your browser (and copy token).

```bash
docker run -it --rm -v$(pwd)/notebooks:/tf/notebooks -v$(pwd)/fruits-360:/tf/notebooks/fruits -p 8888:8888 --dns 8.8.8.8 tensorflow/tensorflow:latest-jupyter
```
