# CMU 15-213 Tiny Shell
This is an attempt to implement CMU 15-213's (Introduction to Computer Systems) Shell Lab.  
More details can be found [here](https://www.cs.cmu.edu/afs/cs/academic/class/15213-s02/www/applications/labs/lab5/shlab.html)  
  

## Directory Structure:  

```
Root
│   
└─── README.md
└─── 
|
└─── src/
       └─── tsh.c : the C-implementation of tiny shell
       └─── tshref: executable of the reference shell
       └─── myspin.c : takes argument <n> and spins for <n> seconds 
       └─── myint.c : spins for <n> seconds and sends SIGINT to itself
       └─── mysplit.c : forks a child that spins for <n> seconds
       └─── myspin.c : takes argument <n> and spins for <n> seconds
|
└─── trace/  
|    └─── trace*.txt : 15 trace files, to control the shell driver 
└─── sdriver.pl : the trace-driven shell driver
└─── tshref.out : example output of the reference shell on all 15 traces

```
## Instructions to build \& run  
1. Clone the repository  
2. In the root, build executables by entering the following:  
```
make clean && make
```
3. Next, the predefined tests(trace files) can be built and tested (on both the reference shell (tshref) as well as the tiny shell (tsh) using):  
```
to test tsh: 	make  test01
to test teshref: make rtest01
```
4. To bring up the shell prompt(after Steps 1 & 2), simply use:
``` 
./src/tsh
```
