# install_OpenCV4
install latest opencv with opecv_contrib CUDA cuDNN etc..
1. Download CUDA Toolkit
https://developer.nvidia.com/cuda-toolkit
2. Install CUDA Toolkit
https://docs.nvidia.com/cuda/cuda-installation-guide-linux/index.html#ubuntu-installation
3. Download  cuDNN
https://developer.nvidia.com/cudnn
4. Install cuDNN
https://docs.nvidia.com/deeplearning/sdk/cudnn-install/index.html
Navigate to your <cudnnpath> directory containing the cuDNN Debian file.
Install the runtime library, for example:
sudo dpkg -i libcudnn8_x.x.x-1+cudax.x_amd64.deb
Install the developer library, for example:
sudo dpkg -i libcudnn8-dev_8.x.x.x-1+cudax.x_amd64.deb
Install the code samples and the cuDNN library documentation, for example:
sudo dpkg -i libcudnn8-doc_8.x.x.x-1+cudax.x_amd64.deb

run 
bash ./install_OpenCV4
it will download latest opencv in ~/Downloads, make it and install.
