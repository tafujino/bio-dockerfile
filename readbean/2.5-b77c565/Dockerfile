FROM ubuntu:20.04
LABEL maintainer="fujino@edu.k.u-tokyo.ac.jp"

WORKDIR /work

ENV DEBIAN_FRONTEND=noninteractive

RUN apt-get update && \
    apt-get install -y git build-essential zlib1g-dev

RUN git clone https://github.com/ruanjue/wtdbg2.git
WORKDIR wtdbg2
RUN git checkout b77c5657c8095412317e4a20fe3668f5bde6b1ac
RUN make

CMD ["/bin/bash"]
