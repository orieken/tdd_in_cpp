# tdd_in_cpp

* reading [Modern C++ Programming with Test-Driven Development](https://pragprog.com/book/lotdd/modern-c-programming-with-test-driven-development)

## Build Status

* travis: [![Build Status](https://travis-ci.com/orieken/tdd_in_cpp.svg?branch=master)](https://travis-ci.com/orieken/tdd_in_cpp)

## Setup on osx

* clone [googletest](https://github.com/google/googletest.git)
* create install dir and change to it
* in install dir run 
```
cmake -DCMAKE_CXX_COMPILER="c++" -DCMAKE_CXX_FLAGS="-std=c++11 -stdlib=libc++" ../
```
* run `make install`
* export paths:
```
echo "export CPLUS_INCLUDE_PATH=/usr/local/include" >> ~/.zshrc 
echo "export LIBRARY_PATH=/usr/local/lib" >> ~/.zshrc
source ~/.zshrc  #reload shell
```

## Build and run
```
make && ./tdd_in_cpp 
```