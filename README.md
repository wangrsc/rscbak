RSC
======

RSC (for Randomly Spherically Constrained single particle cryo-EM) is a stand-alone computer program for vesicle subtraction. It is developed in the
research group of Liguo Wang at both University of Washington and Yale University. It was originally written in Matlab, and is rewritten in Python for distribution.  

The underlying theory of RSC method is given in a scientific publication (https://www.ncbi.nlm.nih.gov/pubmed/19718020). If RSC is useful in your work, please cite this paper.


## Installation


### Please install python3, scipy, numpy, matplotlib if they are not installed
##### In Ubuntu
```
sudo apt install python3-numpy python3-scipy python3-matplotlib
```
##### In Centos
```
sudo yum install python36-pip
sudo python3 -m pip install numpy scipy matplotlib
sudo yum install python36-tkinter
```


### Install git if it is not installed
##### In Ubuntu
```
sudo apt install git
```
##### In Centos
```
sudo yum install git
```

### RSC can be easily installed through
```
git clone https://github.com/wangrsc/rsc
cd rsc
```


###  Test: run the following command and accept default values
```
cd rsc/data
../batch_refit_vesicles.py -f \*dmBIN01.mrc -p 1.056 -m 44 -v dmBIN01.mrc_resub44_screen.txt -c dmBIN01.mrc.ctf -d 1
```