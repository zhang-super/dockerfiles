FROM tensorflow/tensorflow:latest-gpu-py3-jupyter
RUN apt-get update
RUN apt-get -y upgrade
RUN apt-get install -y openssh-server
RUN apt-get install -y net-tools
RUN apt-get install -y iputils-ping
RUN apt-get install -y vim
RUN apt-get install -y sudo
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN echo "PermitRootLogin yes" >> /etc/ssh/sshd_config
RUN pip install --upgrade pip
RUN pip install opencv-python
RUN pip install lxml
RUN pip install pillow
RUN pip install matplotlib
RUN pip install keras
RUN pip install dicom
RUN apt-get install -y cuda