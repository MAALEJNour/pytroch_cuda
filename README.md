
# Docker Image with pytroch_cuda
This docker image contains these Python Packets + Jupyter Notebook: 
- num
- numba
- pandas
- scikit-learn
- matplotlib
- pytorch + CUDA 
- Huggingface Transformer
- accelerate

## Getting Started

These instructions will guide you on how to use this Docker image to run a container with Jupyter Notebook and GPU support.

### Prerequisities

Please make sure that you have nvidia gpu on your computer.

You can verify it by running the following command in your terminal: 
```shell
nvidia-smi
```
If you see a GPU summary like this, you're good to go: 
<img src="https://github.com/MAALEJNour/pytroch_cuda/blob/7e32375b3212852a10d20e893e911c973696162f/cloud_setup_1.jpg" > 

In order to run this container you'll need docker installed: 

* [Windows](https://docs.docker.com/desktop/setup/install/windows-install/)
* [OS X](https://docs.docker.com/desktop/setup/install/mac-install/)
* [Linux](https://docs.docker.com/desktop/setup/install/linux/)
  
If you need help with installation, these YouTube tutorials may help:

* [Windows](https://www.youtube.com/watch?v=-EXlfSsP49A)
* [OS X](https://www.youtube.com/watch?v=-EXlfSsP49A)
* [Linux Ubuntu](https://www.youtube.com/watch?v=cqbh-RneBlk)
### Usage
### Make sure your docker is running before proceeding: 

Ensure Docker Desktop is running before proceeding:
<img src="https://github.com/MAALEJNour/pytroch_cuda/blob/7e32375b3212852a10d20e893e911c973696162f/cloud_setup_3.jpg"> 

#### First Step : Pull the image 

```shell
docker pull maalejnour/pytorch_cuda:latest
```
Wait until the pull is complete: 

<img src="https://github.com/MAALEJNour/pytroch_cuda/blob/7e32375b3212852a10d20e893e911c973696162f/cloud_setup_4.png"> 

After pulling the image, You should see maalejnour/pytorch_cuda:latest in the list:

```shell
docker images
```
<img src="https://github.com/MAALEJNour/pytroch_cuda/blob/7e32375b3212852a10d20e893e911c973696162f/cloud_setup_5.png" > 

#### Second Step : Run the docker container 

To start a container with Jupyter Notebook, use:
```shell
docker run -it -p 8888:8888 --gpus all maalejnour/pytorch_cuda:latest
```
You'll see an output like this with a Jupyter Notebook URL:

<img src="https://github.com/MAALEJNour/pytroch_cuda/blob/9e4b68c4b935121fc9e098390d0cd16738721971/cloud_setup_8.jpg" > 

#### Third Step : Open Jupyter-Notebook

Copy and paste the provided link into your web browser:

<img src = "cloud_setup_6.png" > 


Once opened: 

<img src= "https://github.com/MAALEJNour/pytroch_cuda/blob/c734a251f64531e47f85085cf7e98a3dd23d0a7e/Screenshot%202025-03-16%20135721.png">

* Click New Notebook: 

<img src= "https://github.com/MAALEJNour/pytroch_cuda/blob/4e15183e2365e2f06ba0bfca433bac303d1682d2/Screenshot%202025-03-16%20140159.png">

* Select the PyKernel to start coding: 

<img src= "https://github.com/MAALEJNour/pytroch_cuda/blob/51cfb36941e06c7917028dca8709537e7000f6f9/Screenshot%202025-03-16%20140607.png">

## You can now start coding !

### Example: 

Run the Python code by clicking on the Red Squared Button

<img  src= "cloud_setup_10.png"> 
