# hector_navigation
hector_navigation provides packages related to navigation of unmanned vehicles.
Originally developed for use in Urban Search and Rescue (USAR) environments.

# Installation
```bash
sudo apt-get update && sudo apt-get install libgflags-dev libsuitesparse-dev

mkdir ~/hector_navigation_ws/src/
cd ~/hector_navigation_ws/src/
git clone https://github.com/tu-darmstadt-ros-pkg/hector_slam.git && git checkout noetic-devel
git clone https://github.com/ethz-asl/glog_catkin
git clone https://github.com/catkin/catkin_simple.git
git clone https://github.com/ethz-asl/gflags_catkin
git clone https://github.com/ethz-asl/eigen_catkin.git
git clone https://github.com/ethz-asl/suitesparse
cd ..

catkin_make

cd src/
git clone https://github.com/ethz-asl/ceres_catkin.git
cd ../ && catkin_make

cd src/
git clone https://github.com/tu-darmstadt-ros-pkg/hector_navigation.git && cd ../ && catkin_make
source devel/setup.bash
```
