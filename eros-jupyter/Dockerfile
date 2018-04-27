FROM ros:kinetic-ros-core

RUN apt-get update && apt-get install -y python-pip
RUN pip install jupyter

COPY ./ros_entrypoint.sh /

COPY . /notebooks
WORKDIR /notebooks
