FROM ubuntu:24.04



RUN sudo sed -i.bak 's|http://kr.archive.ubuntu.com/ubuntu/|http://mirror.kakao.com/ubuntu/|g' /etc/apt/sources.list.d/ubuntu.sources
RUN sudo sed -i.bak 's|http://security.ubuntu.com/ubuntu/|http://mirror.kakao.com/ubuntu/|g' /etc/apt/sources.list.d/ubuntu.sources
RUN sudo apt update
RUN sudo apt upgrade

RUN sudo apt-get install python3 python3-pip python3-dev git libssl-dev libffi-dev build-essential
RUN sudo python3 -m pip install --upgrade pip
RUN sudo python3 -m pip install --upgrade pwntools  #can checksec

RUN sudo apt install gdb
RUN sudo git clone https://github.com/pwndbg/pwndbg
RUN cd pwndbg
RUN ./setup.sh
