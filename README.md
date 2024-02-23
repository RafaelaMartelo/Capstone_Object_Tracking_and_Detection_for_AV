# Capstone_Object_Tracking_and_Detection_for_AV
Capstone Project: Object Tracking and Detection in Inclement Weather

Our project focuses on the application of the YOLOv8 model, specifically the YOLOv8 small model, trained on our dataset with labels for cars, persons, and trucks. We introduced data augmentation techniques such as noise and blur to enhance model robustness under various weather conditions. Despite a small and somewhat unbalanced dataset, the performance was reasonably satisfying, highlighting the model's proficiency in identifying key objects with notable precision and recall rates.

### Experiment Configurations
- **Learning Rate Scheduler**: We explored the impact of a cosine learning rate scheduler on the model's generalization capabilities.
- **Batch Size**: The effect of batch sizes 8 and 16 on model performance was assessed, aiming to optimize training efficiency and effectiveness.

### Model Performance Metrics
Our findings, particularly with the 16T configuration, indicated enhanced performance across various metrics, demonstrating the model's effectiveness in critical object detection for autonomous vehicle navigation.

However, the limited dataset size and diversity, along with a significant imbalance favoring car labels, were noted shortcomings. Future work will aim at expanding the dataset to include a broader range of weather scenarios and overall data diversity. Additionally, we plan to explore other features and optimizations during training, resource limitations permitting. Moreover, thorough testing of the application on Streamlit, including edge case analysis, is a priority for future improvements.

For a deeper understanding of the project's objectives, methodologies, and findings, visit our GitHub repository: [Object Detection for Autonomous Vehicles in Inclement Weather GitHub Repository](https://github.com/username/repository-name).

