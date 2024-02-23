# Capstone_Object_Tracking_and_Detection_for_AV
Capstone Project: Object Tracking and Detection in Inclement Weather

## Project Overview
This project explores the application of the YOLOv8 model to enhance object detection capabilities for autonomous vehicles under challenging weather conditions. Utilizing a dataset labeled with cars, persons, and trucks, we employed the YOLOv8 small model, complemented by data augmentation techniques such as noise and blur, to improve detection robustness.

## Repository Structure
- **Data Exploration - CADC Dataset.ipynb**: Offers a detailed exploration of the dataset.
- **Experimentation With Different Models**: Contains a Jupyter notebook that compares YOLOv8 nano, small, and medium models to select the optimal benchmark.
- **Deep Learning Prototype**: Includes a Jupyter notebook detailing the prototype's development process and the decisions that guided its creation.

## Key Experiment Configurations
- **Learning Rate Scheduler**: Investigated the impact of a cosine learning rate scheduler on model generalization.
- **Batch Size**: Evaluated the effects of batch sizes 8 and 16 to optimize model training.

## Model Performance Metrics
Our comprehensive analysis, especially with the 16T configuration, demonstrated significant improvements in model performance:

| Class   | Images | Instances | Precision | Recall | mAP@0.5 | mAP@0.5:0.95 |
|---------|--------|-----------|-----------|--------|---------|--------------|
| All     | 39     | 290       | 86.2%     | 77.5%  | 84.3%   | 58.9%        |
| Car     | 39     | 221       | 85.8%     | 76.5%  | 86.1%   | 60.8%        |
| Person  | 39     | 48        | 78.1%     | 70.8%  | 80.0%   | 45.7%        |
| Truck   | 39     | 21        | 94.7%     | 85.2%  | 86.9%   | 70.2%        |

## Explanation for Selecting the 16T Configuration

The choice of the 16T configuration for our prototype model was informed by a thorough analysis of performance, efficiency, and generalization capabilities. Here's why 16T was the optimal choice:

- **Optimal Performance**: The 16T configuration excelled in accurately detecting objects across classes, with a significant improvement in trucks' detection precision and mAP scores. This enhancement is crucial for navigating adverse weather conditions, demonstrating the model's refined ability to discern crucial objects in complex environments.

- **Balanced Efficiency**: Despite a slight increase in training duration for the 16T configuration, the trade-off was deemed worthwhile due to notable enhancements in detection accuracy and model responsiveness. This balance suggests a robust model design, capable of delivering reliable results while maintaining operational efficiency.

- **Generalization and Inference Speed**: The enabled cosine learning rate scheduler likely contributed to the model's improved generalization, minimizing overfitting risks and bolstering adaptability to diverse weather conditions. Additionally, the maintained efficient inference time is critical for real-time object detection, ensuring prompt processing of images.

## Shortcomings and Future Work

While our project achieved notable success, there are areas requiring further attention to optimize the model's performance fully:

- **Dataset Diversity and Size**: The current dataset, though effective, is limited in size and diversity. Expanding the dataset to include a wider range of inclement weather scenarios and more balanced class distributions will be crucial for enhancing model robustness and reliability.

- **Model Optimization**: Future work will explore additional features and training techniques to optimize the model further. 

- **Comprehensive Testing**: The project's timeline restricted exhaustive testing, particularly on Streamlit. Future efforts will focus on thoroughly testing the application, ensuring it handles edge cases effectively and operates reliably under varied conditions.

## Conclusion

The 16T configuration stands out as a balanced choice, offering high accuracy and practical efficiency, especially in detecting critical object classes under inclement weather conditions. Despite achieving notable precision and recall rates, the project faced challenges such as dataset size and diversity limitations. Future initiatives will aim to address the identified shortcomings, further refining the model to ensure its effectiveness and reliability in real-world autonomous vehicle navigation.

For an in-depth exploration of our methodologies, experiment configurations, and detailed performance metrics, please visit our [GitHub repository](https://github.com/username/repository-name).

## Curious About the Object Detection Demo?

For more details on the project's app demo using the Prototype developed, please visit our GitHub repository: [Object Detection for Autonomous Vehicles in Inclement Weather GitHub Repository - Streamlit App Demo](https://github.com/RafaelaMartelo/object-detection-demo).

I'll provide the app demo link here as a shortcut: [https://object-detection-demoo.streamlit.app/](https://object-detection-demoo.streamlit.app/) shh!

## Contributors

- Rafaela Martelo - [rafaelasofialm98@gmail.com](mailto:rafaelasofialm98@gmail.com)

## License

This project is licensed under the MIT License.
