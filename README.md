# Image-classification-using-Neural-network

Its A Basic Image Classifier using Keras we can the structure i use is similar which is available in keras 
documentation 


Layer (type)                 Output Shape              Param #   
=================================================================
conv2d_33 (Conv2D)           (None, 148, 148, 32)      896       
_________________________________________________________________
activation_31 (Activation)   (None, 148, 148, 32)      0         
_________________________________________________________________
max_pooling2d_29 (MaxPooling (None, 49, 49, 32)        0         
_________________________________________________________________
conv2d_34 (Conv2D)           (None, 47, 47, 32)        9248      
_________________________________________________________________
activation_32 (Activation)   (None, 47, 47, 32)        0         
_________________________________________________________________
max_pooling2d_30 (MaxPooling (None, 23, 23, 32)        0         
_________________________________________________________________
conv2d_35 (Conv2D)           (None, 21, 21, 64)        18496     
_________________________________________________________________
activation_33 (Activation)   (None, 21, 21, 64)        0         
_________________________________________________________________
max_pooling2d_31 (MaxPooling (None, 10, 10, 64)        0         
_________________________________________________________________
flatten_3 (Flatten)          (None, 6400)              0         
_________________________________________________________________
dense_2 (Dense)              (None, 64)                409664    
_________________________________________________________________
activation_34 (Activation)   (None, 64)                0         
_________________________________________________________________
dropout_1 (Dropout)          (None, 64)                0         
_________________________________________________________________
dense_3 (Dense)              (None, 1)                 65        
_________________________________________________________________
activation_35 (Activation)   (None, 1)                 0         
=================================================================
Total params: 438,369
Trainable params: 438,369
Non-trainable params: 0
<br/>
# explaination?-:<br/>


      Image ->  150*150*3 { height -> 150, width->150, depth or RGB -> 3}
      than i apply filter 32 3*3 =>  (148,148,32)
      where 32 is stack of filter basically we found 148 unique position while doing convolution
      =>(I-F)/(S+1)
      =>total number of observation = (3*3*3)*32 -> 864


# what is convolution?
      it is basically moving the filter  over the image with some stride 
      we do dot product of w and x value which lie in the filter and sum it up which give us a single
      value this process is called convolution
      its basically (w.transpose().x +bais)
     
