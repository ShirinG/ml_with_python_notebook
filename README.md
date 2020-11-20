# Modifying pretrained nets - transfer learning

## Daten

https://www.kaggle.com/moltean/fruits

## Docker image pullen

```bash
docker pull tensorflow/tensorflow 
```

## Jupyterlab starten

Run a Jupyter notebook server with your own notebook directory (assumed here to be ~/notebooks). To use it, navigate to localhost:8888 in your browser.

```bash
docker run -it --rm -v$(pwd)/notebooks:/tf/notebooks -v$(pwd)/fruits-360:/tf/notebooks/fruits -p 8888:8888 --dns 8.8.8.8 tensorflow/tensorflow:latest-jupyter
```
