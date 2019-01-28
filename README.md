# A starter kit for Jupyter notebooks and machine learning

![notebooks_screenshot](assets/notebooks.jpg)

## Docker Images

![](https://img.shields.io/docker/automated/wqael/notebooks.svg)
![](https://img.shields.io/docker/build/wqael/notebooks.svg)
![](https://img.shields.io/docker/pulls/wqael/notebooks.svg)
![](https://img.shields.io/docker/stars/wqael/notebooks.svg)

To support both old and new environments, companion [docker images](https://hub.docker.com/r/wqael/notebooks/) are various combinations of
* [python](https://www.python.org/) versions (2.x and 3.x)
* machine learning frameworks ([Keras](https://keras.io/), [Tensorflow](https://www.tensorflow.org/), [PyTorch](https://pytorch.org/))
* [CUDA](https://developer.nvidia.com/cuda-zone) v8 and v9.

All of images include vision-centric libraries, such as
* [jupyter](http://jupyter.org/)
* [OpenCV](https://opencv.org/)
* [scikit-image](http://scikit-image.org/)
* [tensorBoardX](https://github.com/lanpa/tensorboard-pytorch) for [PyTorch](https://pytorch.org/)

Choose a CUDA version that matches the NVidia graphics driver version installed on your system. Here is a compatibility [chart](https://gist.github.com/rlan/258b7c030364735be10c9df277cff5ed).

## Tags

If you are reading this page from [Docker Hub](https://hub.docker.com/r/wqael/notebooks/), the links to Dockefiles will not work. Please go to the github [project page](https://github.com/rlan/notebooks) instead.

### [Caffe](https://caffe2.ai/)

| Tag   | Comment | Dockerfile | Info  |
| ----- | ------- | ---------- | ----  |
| `cuda8dnn7-py2-caffe2-detectron` | For Facebook's [Detectron](https://github.com/facebookresearch/Detectron) | [Dockerfile](docker/cuda8dnn7-py2-caffe2-detectron/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/notebooks:cuda8dnn7-py2-caffe2-detectron.svg) ![](https://images.microbadger.com/badges/commit/wqael/notebooks:cuda8dnn7-py2-caffe2-detectron.svg)](https://microbadger.com/images/wqael/notebooks:cuda8dnn7-py2-caffe2-detectron) |

### [Keras](https://keras.io/) and [Tensorflow](https://www.tensorflow.org/)

| Tag   | Comment | Dockerfile | Info  |
| ----- | ------- | ---------- | ----  |
| `jupyter-keras-tf1.12.0-conda3` | CPU-only | [Dockerfile](docker/jupyter-keras-tf1.12.0-conda3/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/notebooks:jupyter-keras-tf1.12.0-conda3.svg) ![](https://images.microbadger.com/badges/commit/wqael/notebooks:jupyter-keras-tf1.12.0-conda3.svg)](https://microbadger.com/images/wqael/notebooks:jupyter-keras-tf1.12.0-conda3) |
| `jupyter-keras-tf1.12.0-conda2` | CPU-only | [Dockerfile](docker/jupyter-keras-tf1.12.0-conda2/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/notebooks:jupyter-keras-tf1.12.0-conda2.svg) ![](https://images.microbadger.com/badges/commit/wqael/notebooks:jupyter-keras-tf1.12.0-conda2.svg)](https://microbadger.com/images/wqael/notebooks:jupyter-keras-tf1.12.0-conda2) |
| `jupyter-keras-tf1.12.0-conda3-cuda9` | Nvidia Driver >= 384.xx | [Dockerfile](docker/jupyter-keras-tf1.12.0-conda3-cuda9/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/notebooks:jupyter-keras-tf1.12.0-conda3-cuda9.svg) ![](https://images.microbadger.com/badges/commit/wqael/notebooks:jupyter-keras-tf1.12.0-conda3-cuda9.svg)](https://microbadger.com/images/wqael/notebooks:jupyter-keras-tf1.12.0-conda3-cuda9) |
| `jupyter-keras-tf1.12.0-conda2-cuda9` | Nvidia Driver >= 384.xx | [Dockerfile](docker/jupyter-keras-tf1.12.0-conda2-cuda9/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/notebooks:jupyter-keras-tf1.12.0-conda2-cuda9.svg) ![](https://images.microbadger.com/badges/commit/wqael/notebooks:jupyter-keras-tf1.12.0-conda2-cuda9.svg)](https://microbadger.com/images/wqael/notebooks:jupyter-keras-tf1.12.0-conda2-cuda9) |
| `jupyter-keras-tf1.4.1-conda3-cuda8` | Nvidia Driver <= 375.xx | [Dockerfile](docker/jupyter-keras-tf1.4.1-conda3-cuda8/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/notebooks:jupyter-keras-tf1.4.1-conda3-cuda8.svg) ![](https://images.microbadger.com/badges/commit/wqael/notebooks:jupyter-keras-tf1.4.1-conda3-cuda8.svg)](https://microbadger.com/images/wqael/notebooks:jupyter-keras-tf1.4.1-conda3-cuda8) |
| `jupyter-keras-tf1.4.1-conda2-cuda8` | Nvidia Driver <= 375.xx | [Dockerfile](docker/jupyter-keras-tf1.4.1-conda2-cuda8/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/notebooks:jupyter-keras-tf1.4.1-conda2-cuda8.svg) ![](https://images.microbadger.com/badges/commit/wqael/notebooks:jupyter-keras-tf1.4.1-conda2-cuda8.svg)](https://microbadger.com/images/wqael/notebooks:jupyter-keras-tf1.4.1-conda2-cuda8) |

### [PyTorch](https://pytorch.org/)

| Tag   | Comment | Dockerfile | Info  |
| ----- | ------- | ---------- | ----  |
| `jupyter-pytorch1.0-conda3` | CPU-only | [Dockerfile](docker/jupyter-pytorch1.0-conda3/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/notebooks:jupyter-pytorch1.0-conda3.svg) ![](https://images.microbadger.com/badges/commit/wqael/notebooks:jupyter-pytorch1.0-conda3.svg)](https://microbadger.com/images/wqael/notebooks:jupyter-pytorch1.0-conda3) |
| `jupyter-pytorch1.0-conda2` | CPU-only | [Dockerfile](docker/jupyter-pytorch1.0-conda2/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/notebooks:jupyter-pytorch1.0-conda2.svg) ![](https://images.microbadger.com/badges/commit/wqael/notebooks:jupyter-pytorch1.0-conda2.svg)](https://microbadger.com/images/wqael/notebooks:jupyter-pytorch1.0-conda2) |
| `jupyter-pytorch1.0-conda3-cuda9` | Nvidia Driver >= 384.xx | [Dockerfile](docker/jupyter-pytorch1.0-conda3-cuda9/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/notebooks:jupyter-pytorch1.0-conda3-cuda9.svg) ![](https://images.microbadger.com/badges/commit/wqael/notebooks:jupyter-pytorch1.0-conda3-cuda9.svg)](https://microbadger.com/images/wqael/notebooks:jupyter-pytorch1.0-conda3-cuda9) |
| `jupyter-pytorch1.0-conda2-cuda9` | Nvidia Driver >= 384.xx | [Dockerfile](docker/jupyter-pytorch1.0-conda2-cuda9/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/notebooks:jupyter-pytorch1.0-conda2-cuda9.svg) ![](https://images.microbadger.com/badges/commit/wqael/notebooks:jupyter-pytorch1.0-conda2-cuda9.svg)](https://microbadger.com/images/wqael/notebooks:jupyter-pytorch1.0-conda2-cuda9) |
| `jupyter-pytorch1.0-conda3-cuda8` | Nvidia Driver <= 375.xx | [Dockerfile](docker/jupyter-pytorch1.0-conda3-cuda8/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/notebooks:jupyter-pytorch1.0-conda3-cuda8.svg) ![](https://images.microbadger.com/badges/commit/wqael/notebooks:jupyter-pytorch1.0-conda3-cuda8.svg)](https://microbadger.com/images/wqael/notebooks:jupyter-pytorch1.0-conda3-cuda8) |
| `jupyter-pytorch1.0-conda2-cuda8` | Nvidia Driver <= 375.xx | [Dockerfile](docker/jupyter-pytorch1.0-conda2-cuda8/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/notebooks:jupyter-pytorch1.0-conda2-cuda8.svg) ![](https://images.microbadger.com/badges/commit/wqael/notebooks:jupyter-pytorch1.0-conda2-cuda8.svg)](https://microbadger.com/images/wqael/notebooks:jupyter-pytorch1.0-conda2-cuda8) |


### Internal Tags

For intermediate Docker images, from which final images are build from, see [docker/INTERNAL.md](docker/INTERNAL.md).

### Deprecated Tags

For older versions, see [docker/DEPRECATED.md](docker/DEPRECATED.md).


## Usage

**Step 1**: pull pre-built images:

```sh
docker pull wqael/notebooks:<tag>
```

**Step 2**: launch image:

```sh
docker run -it -v $2:/notebooks -p 8888:8888 -p 6006:6006 $1
```

or, for GPU support

```sh
nvidia-docker run -it -v $2:/notebooks -p 8888:8888 -p 6006:6006 $1
```

where:

* `$1` is the tag for a docker image, e.g. `wqael/notebooks:latest`.
* `$2` is the folder containing the notebooks on the host file system, e.g. clone this repo and use `~/notebooks`.


**Step 3**: From the log, copy-and-paste the line similar to the following to your favorite browser:

```
    Copy/paste this URL into your browser when you connect for the first time,
    to login with a token:
        http://localhost:8888/?token=<token string>
```

**Bonus step**: Use next generation [Jupyter](http://jupyterlab.readthedocs.io/en/latest/):

After jupyter home page is loaded, i.e. `http://localhost:8888/tree`, browse to `http://localhost:8888/lab`.

![jupyter_lab_screenshot](assets/jupyter_lab.jpg)

**Step 4**: How to shutdown the docker image:

In the running image terminal, hit Ctrl+C **twice**.
