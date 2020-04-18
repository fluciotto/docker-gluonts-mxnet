FROM python:3.6-slim-stretch

RUN apt update && \
  apt install -y build-essential && \
  apt autoremove -y && rm -rf /var/lib/apt/lists/*

RUN pip install --no-cache-dir  mxnet==1.6.0 gluonts==0.4.2 scikit-learn==0.22.2 tensorflow==2.1.0

RUN apt purge -y build-essential && \
  rm -rf /var/lib/apt/lists/*
