FROM pytorch/pytorch:1.1.0-cuda10.0-cudnn7.5-devel
MAINTAINER zxd
RUN apt-get update
RUN apt-get install vim -y
RUN apt-get install screen -y
RUN apt-get install htop -y 
RUN apt-get install zsh -y
RUN apt-get install openssh-server -y
RUN apt-get install curl -y
RUN apt-get install git -y
WORKDIR /workspace/EagleEye
COPY requirements.txt requirements.txt
RUN pip install pip -U
RUN pip install --upgrade setuptools
RUN pip install -U --ignore-installed wrapt==1.11.1 enum34 simplejson netaddr pyyaml msgpack==0.5.6
RUN pip install -r requirements.txt
