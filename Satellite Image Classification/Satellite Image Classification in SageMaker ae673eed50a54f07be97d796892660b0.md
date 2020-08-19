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
2. Business goal — 
    1. create a model capable of classifying objects such as roads, cars, buildings in satellite images
    2. can be operated in production
    3. can be retrained when new data becomes available
3.