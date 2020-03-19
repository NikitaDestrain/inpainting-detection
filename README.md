# Inpainting Detection
Research UNet CNN architecture for inpainting detection.

This sollution based on [this article](https://arxiv.org/abs/1505.04597).

## Prerequsities
### Infrastructure

* Oracle VM VirtualBox v6.x.x and greater
* Ubuntu 18.04

### Software

* PuTTY (for ssh tunnel creation)
* WinSCP (for copying datasets into VM)
* New fashioned browser like Chrome (for login into Jupyter Notebook)
* Python v3.6.x and greater
* Pip v19.x.x and greater
* Jupyter Notebook in virtual env

### How to guides

* Jupyter Installation guide: [click](https://www.digitalocean.com/community/tutorials/how-to-install-run-connect-to-jupyter-notebook-on-remote-server-ru)
* Python and virtual env installation [click](https://www.digitalocean.com/community/tutorials/how-to-install-python-3-and-set-up-a-programming-environment-on-an-ubuntu-18-04-server)

## Required pip packages
All pacakges should be installed in virual env via `pip install` command

**First of all, update your pip to the last version `python -m pip install --upgrade pip`**

* opencv: `pip install opencv-python`
* numpy: `pip install numpy==1.16.4`
* matplotlib: `pip install matplotlib`
* tensorflow: `pip install tensorflow`

## Draft results

![](https://github.com/NikitaDestrain/inpainting-detection/blob/master/samples/1.png)

## Dataset

* places2
* TBA

Note: I can provide it by request - contact with me via issues or another way.

## Preatrained model

* Batch size: 20
* Epochs: 5
* Validation data size: 200
* Train data size: 1028
