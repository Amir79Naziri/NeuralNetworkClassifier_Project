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
      <a href="usage">Usage</a>
      <ul>
        <li><a href="#usage">Requirements</a></li>
        <li><a href="#run">Run</a></li>
      </ul>
    <li>
      <a href="#Phases">Phases</a>
      <ul>
        <li><a href="#phase1">Preprocess Data</a></li>
        <li><a href="#phase2">Forward Propagation</a></li>
        <li><a href="#phase3">Non-Vectorized Backward Propagetion</a></li>
        <li><a href="#phase4">Vectorized Backward Propagetion</a></li>
        <li><a href="#phase5">Final Test</a></li>
        <li><a href="#phase6">Hyperparameters Analyzing</a></li>
        <li><a href="#phase7">Learning Rate Decay</a></li>
        <li><a href="#phase8">Deeper Network !!!</a></li>
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
this project implements feed forward nerual network from scratch with numpy
the 360 Fruits Dataset has been used for training and testing model.
there are seven phases in this project which complete neural network 
implementation step by step:  

* Preprocess Data
* Forward Propagation
* Non-Vectorized Backward Propagetion
* Vectorized Backward Propagetion
* Final Test
* Hyperparameters Analyzing
* Learning Rate Decay
* Deeper Network !!!  

as input data are images, so there are feature extraction codes 
which can transform image to fixed dimentional
vector, so model uses .pkl extension files as input (not direct images).
first non-vectorized backward propagtion has been impelmented and after that
i changed the backward to vectorized form, thanks for reading.  

feel free to use code ... 
 

<p align="right">(<a href="#top">back to top</a>)</p>

## Usage  
#### Requirements
we used numpy array for increasing speed, then you should install `numpy` library.
```bash
$ pip install numpy
```
also, we used `pygame` for visualizing solving procedure.
```bash
$ pip install pygame
```
#### Run 
```bash
$ python3 csp.py
```

#### Example Run
``` bash
$ python3 csp.py
Which constraint propagation algorithm would you prefer?
 1) MAC
 2) Forward Checking
1
10 10
- 0 - - - - - - - -
- 0 - - - - - 1 - 0
1 - - - 1 0 - - - -
- - - 0 - - - - - 1
- - - - 1 - - - - -
- - - - - - 1 1 - -
- 1 - 1 - - 1 - - -
0 - - - - - - - 0 -
- 1 - - 1 - - 1 0 -
- - - 0 - 0 - - - -
```
then you can see the solving procedure as follows  

![Example Run](./pic/preview.gif)  

<p align="right">(<a href="#top">back to top</a>)</p>

## License

Distributed under the MIT License. See `LICENSE.md` for more information.  

<p align="right">(<a href="#top">back to top</a>)</p>

## Contact
[Amirreza Naziri](https://github.com/Amir79Naziri)  
Email: naziriamirreza@gmail.com  

<p align="right">(<a href="#top">back to top</a>)</p>
