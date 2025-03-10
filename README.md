**Image Forgery Detection System**
The Image Forgery Detection System is an advanced machine learning-based project developed to detect tampering in digital images. In today’s digital world, image manipulation is a growing concern, with forgeries being used for misinformation, fake news, and even cybercrimes. This project aims to address this issue by leveraging Convolutional Neural Networks (CNN) to analyze and classify images as either authentic or forged.

To train and create a model you need download training image sets in to data folder and chage the path for the following files.

1) Extract CNN training patches: as shown in `extract_patches.py`

2) Train CNN: open the `train_net.py` and change DATA_DIR to point to the patches path extracted from the previous step. Run the script, it will save the trained network as shown [here](https://github.com/MudumbaiMadhukanth/Digital-image-forgery-Detection/blob/main/train_net.py)

3) Compute image features: as shown in `feature_extraction.py`. Here you will need to provide the trained CNN as input from the previous step. Change the path in the following [line](https://github.com/MudumbaiMadhukanth/Digital-image-forgery-Detection/blob/main/feature_extraction.py)

4) Run SVM cross-validation: change the features path in `svm_classification.py` at line 5 to point to the latest feature extraction. Run the script.

To run the software download required libraries and execute either *app.py* or *single_imge_test.py* where you upload the image and view the results.
 
