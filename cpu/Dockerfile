FROM python:3.6-slim-stretch

RUN apt update && \
  apt install -y gcc && \
  apt autoremove -y && rm -rf /var/lib/apt/lists/*

RUN pip install --no-cache-dir pydantic==1.4 gluonts==0.4.2 keras==2.3.1 lightgbm==2.3.1 mxnet==1.6.0 scikit-learn==0.22.2 tensorflow==2.1.0 xgboost==1.0.2

RUN apt purge -y gcc
