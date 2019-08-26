# Requirement:

```
python version 3.6 or greater than
keras
Tensorflow
MTCNN
OpenCv
```


## Face_detection_and_recognition

Image Detection system in which we can take the attendance of any college lecture using photos.

In our implementation we are going to be using OpenCV, Sklearn.
## Step 1: Identifying the Faces from Photos or Video
### MTCNN (Multi-task Cascaded Convolutional Networks)

* The MTCNN architecture is reasonably complex to implement. Thankfully, there are open source implementation of the architecture that can be trained as new datasets, as well as pretrained models that can be used directly for Face detection.

* MTCNN is used for detect and align faces where as Facenet is used to create the embedding for the face recognisation.

* Installation of [MTCNN](https://pypi.org/project/mtcnn/).
    
      - pip install mtcnn
      
* 

## Step 2: Recognize image similarity from faces.

* Currently, state of the art face recognition systems use one shot learning. I have come across FaceNet which is the backbone of many open source face recognition system like OpenFace etc.

* FaceNet is introduced in 2015 by Google researchers. It transforms the face into 128D Euclidian space similar to word embedding. Once the FaceNet model having been trained with triplet loss for different classes of faces to capture the similarities and differences between them, the 128 dimensional embedding returned by the FaceNet model can be used to clusters faces effectively. Once such a vector space(embedding) is created, tasks such as face recognition, verification and clustering can be easily implemented using standard techniques with FaceNet embeddings as feature vectors. In a way, distance would be closer for similar faces and further away for non-similar faces.




   




