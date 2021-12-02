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
this project represents a `CSP backtracking algorithm` that can solve `the binary puzzles`,
the binary puzzle consists of an n * n table where n is an even number and
the player must place the numbers zero or one in the empty cells so that:  

* each row and each column must have an equal number of zeros and ones  
* the numbers in each row and column must produce a unique string  
* there should be no more than 2 duplicates in each row and column
  
for example, consider the table in four of the following:
```bash
1   0   0   1
0   1   1   0
1   1   0   0
0   0   1   1
```
1. the number of rows in each row and column is equal to the number of one in that row and column.
2. the string columns 1010, 0110, 0101, and 1001 are unique, and the row strings are similarly unique. 
3. in no row or column are more than two one or two zeros together.  

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
