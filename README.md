# SyReC



# Install python2.7 (in the main terminal (ctrl+alt+t)) 
sudo apt install python-minimal 


# Install python-dev (in the main terminal (ctrl+alt+t))
sudo apt-get install python-dev 


# Install gcc-4.8 and do this (in the main terminal (ctrl+alt+t))
sudo apt-get install gcc-4.8 


## Install g++-4.8 and do this (in the main terminal (ctrl+alt+t))
sudo apt-get install g++-4.8 

# Install PyQt4 (in the main terminal (ctrl+alt+t))
sudo apt-get install python-qt4 

# install libicu48  (in the main terminal (ctrl+alt+t))
wget https://launchpad.net/ubuntu/+archive/primary/+sourcefiles/icu/4.8.1.1-3ubuntu0.10/icu_4.8.1.1.orig.tar.gz 
tar xfz icu_4.8.1.1.orig.tar.gz 
cd icu 
cd source 
./configure 
make 
sudo make install 


# Install cmake 

cd ~/workspace/ (for e.g., inside the main terminal.)

sudo apt-get install build-essential

go to cd /usr/bin 

making gcc-4.8 default gcc

sudo rm gcc 
sudo ln -s gcc-4.8 gcc 

making g++-4.8 default g++

sudo rm g++ 
sudo ln -s g++-4.8 g++ 

come back to cd ~/workspace/ 

wget http://www.cmake.org/files/v3.13/cmake-3.13.4.tar.gz 
tar xf cmake-3.13.4.tar.gz 
cd cmake-3.13.4 
./configure 
make 
sudo make install 


# Run this inside /framework

./build.sh 




# Run this inside /framework/tools   (linking library path)

export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:/usr/local/lib (in terminal (any)) 
export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:/home/checksyrec/Downloads/framework/libs/lib (in terminal (any))




# Run this inside /framework/tools (texting gui)

python syrec_editor.py

chose any .src file from /framework/benchmarks folder


# Run this inside /framework/build/examples (texting the total gate (quantum, number of line (qubits)) cost)

./test_syrec ../../benchmarks/”.src file”
