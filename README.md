# snappy-cpp-example

This project shows cpp how to interact with snappy

#### Snappy Overview
Snappy is a compression/decompression library. It does not aim for maximum compression, or compatibility with any other compresssion library; instead, it aims for very high speeds and reasonable compression.
homepage:[http://google.github.io/snappy/](http://google.github.io/snappy/)
git:[https://github.com/google/snappy](https://github.com/google/snappy)

#### Usage of Snappy
To use Snappy from your own C++ program, include the file "snappy.h" from your calling file, and link against the compiled library.
There are many ways to call Snappy, but the simplest possilble is
```
snappy::Compress(intput.data(), input.size(), &output);
snappy::Uncompress(input.data(), input.size(), &output);
(where "input" and "output" are both instances of stf::string)
```

#### Download Snappy and releated tools
```
git clone https://github.com/google/snappy.git
apt install cmake
apt-get install libsnappy-dev
```

#### Compile and run command
```
g++ -o example ./snappy-example.cpp -I. -L. -lsnappy
./example
```  

#### The output result:
```
input size :736 output size :62
Equal 
```
