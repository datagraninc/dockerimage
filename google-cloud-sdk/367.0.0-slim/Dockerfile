FROM google/cloud-sdk:367.0.0-slim

RUN apt-get update && apt-get install wget gcc make -y
RUN cd /usr/local/src; wget https://ftp.gnu.org/gnu/parallel/parallel-20211022.tar.bz2 && tar jxvf parallel* && cd parallel* && ./configure && make && make install
