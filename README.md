# Tutorial Install OS Jetson Nano
## Step 1. Menginstall OS Jetson Nano, Ikuti panduan pada link dibawah ini
[STEP 1] (https://yunusmuhammad007.medium.com/1-getting-started-with-jetson-nano-developer-kit-a745c9cc598e)
## Step 2. Setup VNC Jetson Nano, Ikuti panduan pada link dibawah ini
[STEP 2] (https://yunusmuhammad007.medium.com/4-setup-vnc-server-pada-jetson-nano-35d3b6121234 (NOTE: Hanya Nomor 1 dan 3 ))
## Step 3. Uninstall Software yang tidak diperlukan, Ikuti panduan pada link dibawah ini
[STEP 3] (https://yunusmuhammad007.medium.com/5-jetson-nano-minimal-os-c50fd1a4ffcd)
## Step 4. Install TensorFlow di Jetson Nano
[STEP 4] (source: https://docs.nvidia.com/deeplearning/frameworks/install-tf-jetson-platform/index.html)
###Before you install TensorFlow for Jetson, ensure you:
1. Sebelum tahap install, kita perlu check JetPack version pada Jetson Nano yang kita gunakan, jalankan command berikut pada terminal
```
sudo apt-cache show nvidia-jetpack
```
2. Install System Package yang dibutuhkan Tensorflow
```
sudo apt-get update
sudo apt-get install libhdf5-serial-dev hdf5-tools libhdf5-dev zlib1g-dev zip libjpeg8-dev liblapack-dev libblas-dev gfortran
```
3. Install dan upgrade pip3
```
sudo apt-get install python3-pip
sudo -H pip3 install -U pip testresources setuptools==49.6.0 
```
4. Install depedency python yang dibutuhkan
```
sudo -H pip3 install -U --no-deps numpy==1.19.4 future==0.18.2 mock==3.0.5 keras_preprocessing==1.1.2 keras_applications==1.0.8 gast==0.4.0 protobuf pybind11 cython pkgconfig packaging
sudo -H H5PY_SETUP_REQUIRES=0 pip3 install -U h5py==3.1.0
```
5. Install Tensorflow
```
sudo pip3 install --extra-index-url https://developer.download.nvidia.com/compute/redist/jp/v46 tensorflow==2.6.0+nv21.11
```
## Step 5. Install package yang dibutuhkan game p9 dan m14
[STEP 5] (Source:)
```
pip3 install nano scipy matplotlib libcanberra-gtk-module opencv-python opencv-contrib-python scikit-learn imutils keras==2.6  numpy==1.19.4

```
## Step 6. Install Driver Razer Kiyo Pro di Jetson Nano, Ikuti panduan pada link dibawah ini
[STEP 6] (https://github.com/dimasalifta/install-driver-razer-kiyo-pro-jetson-nano)
