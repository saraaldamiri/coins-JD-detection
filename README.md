# coins-JD-detection

#Overview:
In this project, we develop a machine learning system designed to detect and accurately count coins. Our goal is to enhance efficiency, reduce errors, and streamline financial processes.

# Objectives:
    * create a deep-learning model for coins detection using roboflow
    * Provide a user-friendly demo using roboflow

# Data Collection:
We collect images for Jordanian currencies(0.05  0.1  0.25  0.5 1  5  10  20  50):

   * capturing images using a camera or mobile device.
   * images from the internet

![1](https://github.com/saraaldamiri/coins-JD-detection/blob/main/data/Screenshot%202024-02-20%20115328.png)

* <b>Sample Images</b>

  ![1](https://github.com/saraaldamiri/coins-JD-detection/blob/main/data/download%20(1).jpeg)
  ![2](https://github.com/saraaldamiri/coins-JD-detection/blob/main/data/download.jpeg)
  ![3](https://github.com/saraaldamiri/coins-JD-detection/blob/main/data/%D8%A7%D9%84%D8%B9%D8%B4%D8%B1%D9%8A%D9%86.png)


# Data Annotation

  * Bounding boxes
    
      ![1](https://github.com/saraaldamiri/coins-JD-detection/blob/main/data/Screenshot%202024-02-21%20115903.png)

  * Polygons
    
    ![1](https://github.com/saraaldamiri/coins-JD-detection/blob/main/data/Screenshot%202024-02-21%20115925.png)



# Preprocessing steps:
In all Models, we do the same general preprocessing steps that are:

* Image resizing Below are the target sizes used for resizing images for different models:
  
| Model         | Target Size Used |
|---------------|------------------|
|V3             | 1024*1024        |
|v12            | 640*412          |
|v15            | 640*640          |

* Data Augmentation.
  We split the data into training and testing sets with an 80:20 ratio, then we apply data augmentation exclusively to the training data.

  Data augmentation is a technique used to enhance the size and diversity of a training dataset by applying various transformations to existing images. This process is pivotal for 
  improving the generalization and robustness of trained models, as it exposes them to a wider range of input variations.

  We apply different data augmentation techniques to each model, and we will provide the specific augmentation process with each model."

  * example of data augmentation
    
      ![1](https://github.com/saraaldamiri/coins-JD-detection/blob/main/data/Screenshot%202024-02-21%20120724.png)

# Modeling

## v3 with map(77.4%)
  * Mixed annotation 
  * small dataset

     ![1](https://github.com/saraaldamiri/coins-JD-detection/blob/main/data/Screenshot%202024-02-21%20131522.png)
     ![2](https://github.com/saraaldamiri/coins-JD-detection/blob/main/data/Screenshot%202024-02-21%20131547.png)
     ![3](https://github.com/saraaldamiri/coins-JD-detection/blob/main/data/Screenshot%202024-02-21%20131236.png)
     ![4](https://github.com/saraaldamiri/coins-JD-detection/blob/main/data/Screenshot%202024-02-21%20131444.png)

  * example of result
    
    ![1](https://github.com/saraaldamiri/coins-JD-detection/blob/main/data/Screenshot%202024-02-21%20135210.png)
    ![2](https://github.com/saraaldamiri/coins-JD-detection/blob/main/data/Screenshot%202024-02-21%20135143.png)
    ![3](https://github.com/saraaldamiri/coins-JD-detection/blob/main/data/Screenshot%202024-02-21%20140322.png)


## v12 with map(77.4%)





