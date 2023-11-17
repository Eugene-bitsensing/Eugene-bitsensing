- 👋 Hi, I’m @Eugene-bitsensing
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
Eugene-bitsensing/Eugene-bitsensing is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->




git clone --recursive git@github.com:bitsensing/atm220_sw.git

git submodule deinit -f tensorrt
git rm ./tensorrt
git submodule add git@github.com:bitsensing/tensorrt.git tensorrt
git checkout feature/PA-171_bug_fix 

 sudo apt-get install update cmake
 sudo apt install libboost-all-dev

sudo apt-get install build-essential gcc make cmake cmake-gui cmake-curses-gui
sudo apt-get install fakeroot devscripts dh-make lsb-releaselibssl-dev
apt-get install doxygen graphviz

# run in ~/ 
git clone https://github.com/eclipse/paho.mqtt.c.git
mkdir /tmp/build.paho ; cd /tmp/build.paho
cmake -DPAHO_WITH_SSL=TRUE -DPAHO_BUILD_DOCUMENTATION=TRUE \
    -DPAHO_BUILD_SAMPLES=TRUE ~/paho.mqtt.c

ccmake ~/paho.mqtt.c
sudo cmake --build . --target install

sudo apt-get install libgtk-3-dev
sudo apt-get install pkg-config

#argus custom install -> need to change include dir in atm220_sw/eCam_argus_camera/argus/cmake/findargus.cmake 

mkdir atm220_sw/eCam_argus_camera/argus/build
cd atm220_sw/eCam_argus_camera/argus/build

cmake ..
cd ..
make -j4

sudo make install 

#wget https://downloads.apache.org/kafka/3.6.0/kafka_2.13-3.6.0.tgz
#tar -xvzf ./kafka_2.13-3.6.0.tgz
#
#git clone https://github.com/apache/kafka.git
#sudo apt-get install openjdk-11-jdk
#sudo apt-get install curl
sudo apt install librdkafka-dev

sudo apt-get install libgstreamer1.0-dev libgstreamer-plugins-base1.0-dev libgstreamer-plugins-bad1.0-dev gstreamer1.0-plugins-base gstreamer1.0-plugins-good gstreamer1.0-plugins-bad gstreamer1.0-plugins-ugly gstreamer1.0-libav gstreamer1.0-doc gstreamer1.0-tools gstreamer1.0-x gstreamer1.0-alsa gstreamer1.0-gl gstreamer1.0-gtk3 gstreamer1.0-qt5 gstreamer1.0-pulseaudio

sudo apt-get install -y libgstrtspserver-1.0-dev

git clone https://github.com/confluentinc/librdkafka.git
git checkout tags/v1.8.2-RC5
./configure --install-deps
  make
  sudo make install


 grep -r workspace/project *
