# DETECTRON2 local windows 10 setup

## This setup can be used for prediction or model testing

*install python 3.7.0 (as tested) : (https://www.python.org/ftp/python/3.7.0/python-3.7.0-amd64.exe " python 3.7.0 exe")
* install visual studio  for C++ 14.0: (https://visualstudio.microsoft.com/thank-you-downloading-visual-studio/?sku=BuildTools&rel=16)
* install CUDA: (https://addiguru.atlassian.net/wiki/spaces/DS/pages/66289665/Auto+Start+XAMPP+for+Windows+10)
* if wants to install in Virtualenv : 
```
virtualenv myenv
cd myenv/Scripts
activate
```
* run to install packages :
```
pip install tensorflow-cpu==2.2

pip install torch==1.7.0+cu101 torchvision==0.8.1+cu101 torchaudio===0.7.0 -f https://download.pytorch.org/whl/torch_stable.html


pip install git+https://github.com/facebookresearch/fvcore

cd ../..

git clone https://github.com/conansherry/detectron2.git
pip install -e detectron2
pip install opencv-python
pip install pycocotools
```
* Test installation:
```
python detectron2/tests/test_boxes.py
```
