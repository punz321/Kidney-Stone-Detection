# Kidney-Stone-Detection
In this project, we'll be using YOLOv9 to detect stones in kidneys

# Dataset
In this study, we used CT KIDNEY dataset from Kaggle, which was in turn taken from PACS (Picture Archiving and Communication System) and office work at a hospital in Dhaka, Bangladesh, where patients were diagnosed with kidney cancer, cyst, normal, or stone. All subjects in the data voluntarily participated in the research experiment and their informed consent was confirmed before data collection. The dataset contains 12,466 unique pieces of data, of which 3,709 were normal, 5,077 were normal, 1,377 were stones, and 2,283 were tumors. We manually annotated the images to train the model on the kidney images.

# Model Architecture
YOLOv9 builds upon the YOLOv7 models and utilizes a new concept called Programmable Gradient Information (PGI) and Generalized Efficient Layer Aggregation Network (GELAN) [1] (yolov9 official reference paper). It tackles the problem of information loss during training.
- PGI
> It is a new technique that adds a special path to the model that helps it learn better during the training process.
>The path ensures the model gets accurate updates.
- GELAN
> It is an architecture designed for optimal parameter usage, computational efficiency, and improved accuracy.
> It allows us to choose suitable computational blocks for different devices that we deploy the model on.

# Results
The YOLOv9 model achieved a mean Average Precision (mAP) of 85% on the test dataset, indicating its effectiveness in object detection tasks. The model demonstrated high precision and recall rates, with precision at 82% and recall at 84%. These results underscore the YOLOv9 model's ability to accurately detect and localize objects in images while maintaining a low false positive rate.

Not yet deployed the model, but in the process

Will release the annotated dataset soon!

# Notes
> Use your own API key in kaggle.json file

> Update the paths of train and test folder in data.yaml file
