# ssd_model
The programs in this repository train and use a Single Shot MultiBox Detector to take an image and draw bounding boxes around hands contained in the image. The network is based on the VGG-16 model and uses the approach described in this https://arxiv.org/abs/1512.02325 paper by Wei Liu et al.

Hand DataSets can be downloaded from here - <br/>
  1)http://www.robots.ox.ac.uk/~vgg/data/hands/ <br/>
  2)http://vision.soic.indiana.edu/projects/egohands/ <br/>
 
 
You then need to preprocess the dataset before you can train the model on it.<br/>
  ./process_dataset.py <br/>

You can then train the whole thing. It will take around 150 to 200 epochs to get good results.<br/>
  ./train.py <br/>
  
If you want to make detection basing on the inference model, check out: <br/>
  ./detect.py <br/>
