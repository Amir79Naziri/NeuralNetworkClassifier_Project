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
        <li><a href="#Phase1">Preprocess Data</a></li>
        <li><a href="#Phase2">Forward Propagation</a></li>
        <li><a href="#Phase3">Non-Vectorized Backward Propagetion</a></li>
        <li><a href="#Phase4">Vectorized Backward Propagetion</a></li>
        <li><a href="#Phase5">Final Test</a></li>
        <li><a href="#Phase6">Hyperparameters Analyzing</a></li>
        <li><a href="#Phase7">Learning Rate Decay</a></li>
        <li><a href="#Phase8">Deeper Network !!!</a></li>
      </ul>
    </li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li> 
  </ol>
</details>

## About The Project
This project implements a `feed-forward neural network` from scratch with `numpy` and uses the `360 Fruits` Dataset as a training and testing model. there are seven phases in this project which complete neural network implementation step by step, which includes the following steps  

* [Preprocess Data](#Phase1)
* [Forward Propagation](#Phase2)
* [Non-Vectorized Backward Propagetion](#Phase3)
* [Vectorized Backward Propagetion](#Phase4)
* [Final Test](#Phase5)
* [Hyperparameters Analyzing](#Phase6)
* [Learning Rate Decay](#Phase7)
* [Deeper Network !!!](#Phase8)

As input data are images, so there are some feature extraction codes that can transform images into fixed dimensional vectors, so the model uses `.pkl` extension files as input (not direct images). In the beginning, `non-vectorized` `backward propagation` will be implemented, and after that implementation will be changed to `vectorized` backward propagation. 

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
and you should install `tqdm` for better experince (you can delete it from code if you want)
```bash
$ pip install tqdm
```
__(optional)__  
if you want to run feature extraction codes yourself, please install `scikit-image` too
```bash
$ pip install scikit-image
```

### Run 
Run all cells in order, but you should run phase 7 before running the train function's cell at phase 3.

<p align="right">(<a href="#top">back to top</a>)</p>

## Phases  

<h3 id="Phase1">Preprocess Data</h3>  

In this phase data is transformed from images into vectors, at beginning feature extraction reads all images and with the use of `histogram` function and number of 360 `bins`, images are transformed into vectors, then features with specific `standard deviation` are deleted, and finally, data is ready!  

<h3 id="Phase2">Forward Propagation</h3>  
  
In this phase `forward function` is implemented and weights and biases are initialized, also the test function is implemented for testing the `accuracy` of the model. As `activation function`, this model uses `sigmoid` for all layers.  


<h3 id="Phase3">Non-Vectorized Backward Propagetion</h3>  
In this phase `nonvectorized backward function` is implemented, but it is so slow. 


<h3 id="Phase4">Vectorized Backward Propagetion</h3>  
In this phase `vectorized backward function` is implemented, as you can see it is super fast.

<h3 id="Phase5">Final Test</h3>  


<h3 id="Phase6">Hyperparameters Analyzing</h3>  


<h3 id="Phase7">Learning Rate Decay</h3>  
I used a custom learning decay for improving convergence.  
```python
class LR_Decay:
    def __init__(self, initial_lr, k):
        self.initial_lr = initial_lr
        self.t = 0
        self.k = k
        
    def step(self):
        value = self.initial_lr * np.exp(-self.k * self.t)
        self.t += 1
        return max(value, 1)
```

<h3 id="Phase8">Deeper Network !!!</h3>  
In the last phase, 3 fruits were added to the dataset, so there are seven fruits and also we need Deeper Model !!!

###### warning: feel free to add more fruits to the dataset, but you should modify feature extraction a little bit and make your model more complex.


<p align="right">(<a href="#top">back to top</a>)</p>

## License

Distributed under the MIT license. See `LICENSE.md` for more information.  

<p align="right">(<a href="#top">back to top</a>)</p>

## Contact
[Amirreza Naziri](https://github.com/Amir79Naziri)  
Email: naziriamirreza@gmail.com  

<p align="right">(<a href="#top">back to top</a>)</p>
