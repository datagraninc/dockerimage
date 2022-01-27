FROM python:3.8-bullseye

ENV DEBIAN_FRONTEND=noninteractive
RUN apt-get update -y  && apt-get upgrade -y
RUN apt-get install locales -y && locale-gen en_US.UTF-8
ENV LANG=en_US.UTF-8 \
    LANGUAGE=en_US:en \
    LC_ALL=en_US.UTF-8

RUN /usr/local/bin/python -m pip install --upgrade pip
RUN pip install sklearn numpy pandas tensorflow scipy keras statsmodels gensim torch xgboost click pyarrow joblib dill cloudpickle