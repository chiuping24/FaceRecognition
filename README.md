# FaceRecognition
Face recognition with TensorFlow
1. Python 3.5.2 :: Anaconda 4.1.1 (64-bit)
2. windows 10
3. tensorflow CPU version

```
$ python
$ import tensorflow as tf
$ print(tf.__version__)
1.3.0
```
4. [good reference of face recognition with Tensorflow](http://www.jianshu.com/p/3e5ddc44aa56)
5. [good introduction of Convolutional neural network of Tensorflow](http://arbu00.blogspot.tw/2017/03/2-tensorflowconvolutional-neural.html)

#### Brief introduction of CNN of Tensorflow
區域感知域(Local Receptive field)，卷積(Convolutional )，池化(pooling)  
CNN使用過濾器(filters)增強與該局部圖形空間的相關性，然後堆疊許多這樣子的層   

1. Convolution layer:  
* filter size/ number
* 搭配適當的convolution layer 可使training model效率和結果提升
* full connection layer number 可被調控   
2. Pooling  
3. Default TensorFlow model saving in python  
* .ckpt: (index) checkpoint 包含模型中所有variable  
* model.ckpt.meta: the graph strucutre of model  
* 輸出單個文件(包含模型架構與權重 .pb) 方便其他使用ex: C++  
* tf.train.write_graph(session.graph_def, "/tmp/load", "test.pb", False) #proto  
* 
