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

![](https://github.com/NikitaDestrain/inpainting-detection/blob/master/samples/2.png)

![](https://github.com/NikitaDestrain/inpainting-detection/blob/master/samples/3.png)

## Dataset

* places2
* TBA

Note: I can provide it by request - contact with me via issues or another way.

## Pretrained model

### DFNet_UnetW.h5
* Mask form: rectangle
* Batch size: 20
* Epochs: 5
* Validation data size: 200
* Train data size: 1028

### DFNet_UnetW_3batch.h5
* Mask form: rectangle
* Batch size: 3
* Epochs: 10
* Validation data size: 400
* Train data size: 1028

### DFNet_UnetW_5_10.h5
* Mask form: rectangle
* Batch size: 5
* Epochs: 10
* Validation data size: 400
* Train data size: 1028

### DFNet_UnetW_5_10_ellipse.h5 - no way results for 0.3 result of CNN
* Mask form: ellipse
* Batch size: 4
* Epochs: 10
* Validation data size: 400
* Train data size: 1028

### Context_Encoder_UnetW_5_10.h5 - 100% detection, because we have inpainting in the same place for all images 
* Mask form: rectangle
* Batch size: 5
* Epochs: 10
* Validation data size: 350
* Train data size: 1002
