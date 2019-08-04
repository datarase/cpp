# C++ REST DEMO 
#compile command

g++ -o restapi_test httphandler.cpp  strutil.cpp  restapi.cpp execute.cpp -I /usr/local/lib -lmicrohttpd /usr/lib/x86_64-linux-gnu/libboost_regex.a -lpthread

#To Run the server program


./restapi_test 1345

To invoke http rest api requests as below:



http://127.0.0.1:1345/diskinfo


http://127.0.0.1:1345/sysinfo?fields=memory

Dependancies:
1) Install boost on ubuntu (Boost property tree is used for generating XML/JSON data)

sudo apt-get install libboost-all-dev

2) Install libmicrohttpd on ubuntu

sudo apt-get update

sudo apt-get install libmicrohttpd-dev


