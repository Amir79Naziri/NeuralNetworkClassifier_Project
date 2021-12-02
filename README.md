<div align="center">
  
  <h1 align="center">360 Fruits Classifier</h1>
</div>

<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
    </li>
    <li>
      <a href="Usage">Usage</a>
      <ul>
        <li><a href="#Requirements">Requirements</a></li>
        <li><a href="#Run">Run</a></li>
      </ul>
    <li>
      <a href="#Phases">Phases</a>
      <ul>
        <li><a href="#Preprocess Data">Preprocess Data</a></li>
        <li><a href="#Forward Propagation">Forward Propagation</a></li>
        <li><a href="#Non-Vectorized Backward Propagetion">Non-Vectorized Backward Propagetion</a></li>
        <li><a href="#Vectorized Backward Propagetion">Vectorized Backward Propagetion</a></li>
        <li><a href="#Final Test">Final Test</a></li>
        <li><a href="#Hyperparameters Analyzing">Hyperparameters Analyzing</a></li>
        <li><a href="#Learning Rate Decay">Learning Rate Decay</a></li>
        <li><a href="#Deeper Network !!!">Deeper Network !!!</a></li>
          <ul>
            <li><a href="#phase8-1">Preprocess Data</a></li>
            <li><a href="#phase8-2">Train and Test</a></li>
          </ul>
      </ul>
    </li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li> 
  </ol>
</details>

## About The Project
This project implements a `feed-forward neural network` from scratch with `numpy` and uses the `360 Fruits` Dataset as a training and testing model. there are seven phases in this project which complete neural network implementation step by step, which includes the following steps  

* [Preprocess Data](#Preprocess Data)
* [Forward Propagation](#Forward Propagation)
* [Non-Vectorized Backward Propagetion](#Non-Vectorized Backward Propagetion)
* [Vectorized Backward Propagetion](#Vectorized Backward Propagetion)
* [Final Test](#Final Test)
* [Hyperparameters Analyzing](#Hyperparameters Analyzing)
* [Learning Rate Decay](#Learning Rate Decay)
* [Deeper Network !!!](#Deeper Network !!!)

As input data are images, so there are some feature extraction codes that can transform images into fixed dimensional vectors, so the model uses .pkl extension files as input (not direct images). In the beginning, non-vectorized backward propagation was implemented, and after that implementation changed from the vectorized backward propagation to vectorized form.  

feel free to use code :wink:  

###### Thanks for your reading :heart:
 

<p align="right">(<a href="#top">back to top</a>)</p>

## Usage  
### Requirements
Project uses numpy array for increasing speed and Linear algebra, then you should install `numpy` library
```bash
$ pip install numpy
```
also, project needs `matplotlib` for visualizing plots
```bash
$ pip install matplotlib
```
and you should install `tqdm` for better experince(you can delete it from code if you want)
```bash
$ pip install tqdm
```
__(optional)__  
if you want to run feature extraction codes yourself, please install `scikit-image` too
```bash
$ pip install scikit-image
```

### Run 
Run all cells in order, but you should run phase 7 before running the train function cell at phase 3.

<p align="right">(<a href="#top">back to top</a>)</p>

## Phases

### Preprocess Data
### Forward Propagation)
### Non-Vectorized Backward Propagetion)
### Vectorized Backward Propagetion)
### Final Test)
### Hyperparameters Analyzing)
### Learning Rate Decay)
### Deeper Network !!!)

## License

Distributed under the MIT license. See `LICENSE.md` for more information.  

<p align="right">(<a href="#top">back to top</a>)</p>

## Contact
[Amirreza Naziri](https://github.com/Amir79Naziri)  
Email: naziriamirreza@gmail.com  

<p align="right">(<a href="#top">back to top</a>)</p>
