FROM nvidia/cuda:9.0-cudnn7-devel-ubuntu16.04
RUN apt-get update
RUN apt-get -y upgrade
RUN apt-get install -y openssh-server
RUN apt-get install -y net-tools
RUN apt-get install -y iputils-ping
RUN apt-get install -y vim
RUN apt-get install -y sudo
RUN apt-get install -y python-pip
RUN apt-get install -y wget
RUN python -m pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN echo "PermitRootLogin yes" >> /etc/ssh/sshd_config
RUN pip install numpy
RUN pip install tensorflow-gpu==1.11.0
RUN pip install opencv-python
RUN pip install lxml
RUN pip install pillow
RUN pip install matplotlib==2
RUN pip install keras
RUN pip install dicom