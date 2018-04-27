FROM ros:kinetic-ros-core

RUN apt-get update

COPY ./ros_entrypoint.sh /
COPY . /catkin_ws
RUN ./ros_entrypoint.sh && cd /catkin_ws && rosdep install --from-paths src --ignore-src -r -y
