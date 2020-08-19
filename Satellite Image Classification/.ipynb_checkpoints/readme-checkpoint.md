# Satellite Image Classification

This lecture was taken from Satellite Image Classification in SageMaker [Learning Library](https://www.aws.training/Details/Video?id=27231) 

- ML process
    - Understand the business problem and goal
    - Frame the problem as ML model
        - Data wrangling {Data collection, data integration, data preparation and cleaning}
        - Data visualization and analysis
        - feature engineering
        - model training and parameter turning
        - model evaluation
    - Are the business goal met after framing the ML model? Re-do or deploy?
        - No —> **feature** augmentation or **data** augmentation
        - Yes —> model deployment
    - In the deployment
        - Predictions can be gathered
        - by monitoring and debug the model
        - If possible, we can do re-training with new acquired data.
    - 

### Satellite Image Classification

Let us do it based on the ML process above

1. Business problem — identifying and counting specific objects in an image is a human cognition task that is both **costly** and **inefficient**
2. Business goal — 72% accuracy
    1. create a model capable of classifying objects such as roads, cars, buildings in satellite images
    2. can be operated in production
    3. can be retrained when new data becomes available
3. Frame the ML model
    1. Data collection from various satellite image' sources.
    2. Use open-source API to label the images. 
    3. Divide the data to training and validation set (80,20)
    4. Use data augmentation to create more datas such as rotating the images to 30,60 and 90 degress to increase the varience and to prevent overfitting. 
        
### Dataset

DigitalGlobe

   1. stored in AWS' cloud
   2. 100 petabytes of iamge library
   3. use SageMaker to easily host jupyter notebooks for iamge processing.
   
There are many types of data for processing. For this particular problem, a classification problem, there are certain criterias for the dataset;
- An adequate zoom for building, cars and road classification
    
### Convolution fundamentals

- Filters detect patterns, edges, shapes, textures etc. It is a small matrix with given number of columns and rows.
- Must have same depth of input data -- because it computes a dot product with a chunk of the image. 
- Features:
    - Low-level features ( similar to edge detection)
    - Mid-level features – shapes 
    - High-level features – the area itself or the object in 


***However, due to large size of satellite images, the classification will not take place on the computer.


#### Resources
[Label-maker](https://github.com/developmentseed/label-maker)