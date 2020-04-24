FROM nvidia/cuda:10.2-runtime

# RUN apt update && \
#   apt install -y gcc python3.6 python3-pip
RUN apt update && \
  apt install -y gcc python3-pip

RUN pip3 install --upgrade pip
RUN pip3 install --no-cache-dir pydantic==1.4 gluonts==0.4.2 mxnet-cu102==1.6.0 scikit-learn==0.22.2 tensorflow==2.1.0

RUN apt purge -y gcc
