# DETECTRON2 local windows 10 setup for CPU

## This setup can be used for prediction or model testing



* install python 3.7.0 (as tested) : [python 3.7.0 exe](https://www.python.org/ftp/python/3.7.0/python-3.7.0-amd64.exe)
* install visual studio  for C++ 14.0: [Click here](https://visualstudio.microsoft.com/thank-you-downloading-visual-studio/?sku=BuildTools&rel=16)
  (make sure to select C++ then select 2 MSVC pckage from bottom of default selected list)
* install CUDA 10.1: [link](https://developer.nvidia.com/cuda-10.1-download-archive-base?target_os=Windows&target_arch=x86_64&target_version=10&target_type=exelocal)
  * if want to install in Virtualenv : 
  ```
  virtualenv myenv
  cd myenv/Scripts
  activate
  ```
* run to install packages :
```
pip install tensorflow-cpu==2.2
pip install torch==1.7.0+cu101 torchvision==0.8.1+cu101 torchaudio===0.7.0 -f https://download.pytorch.org/whl/torch_stable.html
pip install opencv-python
pip install pycocotools
pip install git+https://github.com/facebookresearch/fvcore
```
  * if installing in virtual env(execute if u want access to detectron2 folder)
  ```
  cd ../..
  ```
* Clone detectron2 repo & run setup
```
git clone https://github.com/facebookresearch/detectron2.git
pip install -e detectron2

```
