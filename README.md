# Machine Learning

###### Transfer learning using tensorflow VGG16 image classification model
We have used the transfer learning VGG16 classification model to classify our own FOOD dataset. After creating trasnfer codes using the existing model, we have added fully connected and activation layers to perform a higher layer classfication on our GOT dataset.

The model reaches validation accuracy of ~82% in 100 Epochs and is extremely fast!
It shows how transfer learning can be used to solve classification tasks, by building sleek and prodigiously fast models.

Steps:
* Download Dataset 
    [food11-image-dataset] (https://www.kaggle.com/trolukovich/food11-image-dataset “food11-image-dataset”)
    [indonesian food] (https://www.dropbox.com/sh/88stvg9krafl7z8/AAC97IdMbHe7ksp8Cc8I08K2a?dl=0 “Food Dataset”)
* Upload dataset in Google Drive (name folder: Gdrive)

- Run the model using file "capstone.py"


Overview:
transferModel file imports createTransferCodes file
createTransferCodes does following things:
download the VGG16 model data (.npy file)
apply transformations if required
create transfer codes and store them in the project directory
Note: Images transformations are created if number of images for any class are less than 500

References:
Image transformation: https://github.com/vxy10/ImageAugmentation
VGG16 Model: https://github.com/machrisaa/tensorflow-vgg
Progress bar: https://blog.shichao.io/2012/10/04/progress_speed_indicator_for_urlretrieve_in_python.html
