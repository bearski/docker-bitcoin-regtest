FROM ubuntu:trusty

RUN sudo apt-get -y update
RUN sudo apt-get install -y python-software-properties 

RUN sudo add-apt-repository ppa:bitcoin/bitcoin
RUN sudo apt-get update
RUN sudo apt-get install -y bitcoind

RUN sudo mkdir ~/.bitcoin
RUN sudo echo "rpcuser=test\nrpcpassword=test\n" > ~/.bitcoin/bitcoin.conf

RUN sudo echo "alias rt='bitcoind -regtest'" >> ~/.bashrc
