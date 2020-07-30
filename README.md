# install_OpenCV4
install latest opencv with opecv_contrib CUDA cuDNN etc..

1. Download CUDA Toolkit
https://developer.nvidia.com/cuda-toolkit

2. Install CUDA Toolkit
https://docs.nvidia.com/cuda/cuda-installation-guide-linux/index.html#ubuntu-installation
Perform the pre-installation actions.
Install repository meta-data
$ sudo dpkg -i cuda-repo-<distro>_<version>_<architecture>.deb
Installing the CUDA public GPG key
When installing using the local repo:

$ sudo apt-key add /var/cuda-repo-<version>/7fa2af80.pub
When installing using network repo on Ubuntu 20.04/18.04:

$ sudo apt-key adv --fetch-keys https://developer.download.nvidia.com/compute/cuda/repos/<distro>/<architecture>/7fa2af80.pub
When installing using network repo on Ubuntu 16.04:

$ sudo apt-key adv --fetch-keys http://developer.download.nvidia.com/compute/cuda/repos/<distro>/<architecture>/7fa2af80.pub
Pin file to prioritize CUDA repository:

$ wget https://developer.download.nvidia.com/compute/cuda/repos/<distro>/<architecture>/cuda-<distro>.pin
$ sudo mv cuda-<distro>.pin /etc/apt/preferences.d/cuda-repository-pin-600
Update the Apt repository cache
$ sudo apt-get update
Install CUDA
$ sudo apt-get install cuda
Perform the post-installation actions.
  
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

5. run 

bash ./install_OpenCV4

it will download latest opencv in ~/Downloads, make it and install.
