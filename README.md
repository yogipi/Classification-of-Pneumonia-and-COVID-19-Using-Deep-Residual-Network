# Classification-of-Pneumonia-and-COVID-19-Using-Deep-Residual-Network
The train and validation dataset that I used came from research conducted by Daniel S. Kermany, Michael Goldbaum, et al. and research conducted by Muhammad E. H. Chowdhury, Tawsifur Rahman, Amith Khandakar, et al. Meanwhile, for the test dataset obtained from the research of Amanullah Ashraf, et al. From the dataset he shared, I took the train dataset and validated 999 x-ray images of pneumonia, 999 positive x-ray images for COVID-19, and 999 normal x-ray images. Meanwhile, for the pneumonia and COVID-19 test data, I took 333 x-ray images.

The dataset I use is shared in this folder: https://drive.google.com/drive/folders/1nY6b6gYrhM4sP38vZdAvd3iHDg3nVNKV?usp=sharing

The entire dataset can be viewed here: 
https://www.kaggle.com/datasets/tawsifurrahman/covid19-radiography-database
https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia 
https://www.kaggle.com/datasets/amanullahasraf/covid19-pneumonia-normal-chest-xray-pa-dataset  

Raw images are different scale images in three different formats, namely .jpg, .png, and .jpeg. Raw images with different scales and formats cannot be entered into the model at the same time. So, the dataset must be preprocessed first by converting it to float by dividing each image pixel value by the maximum pixel value of the image. Using this preprocessing the image will have a similar pixel scale i.e., 224x224 with a 32-bit float type that can be entered into the system model.
