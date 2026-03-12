# Fashion Computer Vision Classification Prototype

Computer vision prototype for automated fashion item classification into 8 retail categories using PyTorch and Google Colab.

## Executive Summary
This project is an applied computer vision prototype built to classify fashion images into 8 retail product categories. The objective was to evaluate whether machine learning could support automated product tagging and improve downstream merchandising intelligence in a retail setting.

Three model approaches were explored:
- Multilayer Perceptron (MLP)
- VGG16 implemented from scratch
- Pre-trained VGG16

The project included dataset preparation, custom test data loading, image preprocessing, hyperparameter tuning, TensorBoard experiment tracking, and performance evaluation using validation accuracy, confusion matrices, and mean average precision (mAP).

## Business Problem
Fashion retailers and digital commerce teams often rely on manual catalog tagging, which is time-consuming and inconsistent. A scalable image classification workflow can help automate product categorisation, support trend visibility, and improve recommendation workflows such as “Complete the Look.”

## Role & Scope
This project was executed end-to-end as an individual machine learning build. Scope included:
- defining the classification problem
- preparing the data pipeline
- implementing and training multiple architectures
- evaluating model performance
- analyzing class-level error patterns
- interpreting technical findings through a product and business lens

## Technical Stack
- Python
- PyTorch
- Google Colab
- NumPy
- Matplotlib
- Seaborn
- TensorBoard
- scikit-learn

## Classification Scope
The model classifies images into 8 fashion categories:
- Accessories
- Jackets
- Jeans
- Knitwear
- Shirts
- Shoes
- Shorts
- Tees

## Results Overview
The prototype progressed from a lightweight MLP baseline to stronger CNN-based performance, with the **pre-trained VGG16 model delivering the strongest results**. This suggests that transfer learning was more effective than both the MLP baseline and the from-scratch VGG16 approach for this fashion classification task.

![Results Overview](https://github.com/Korra1234/fashion-computer-vision-classification/blob/338c9977e47e21dae423f21fc5889af2de7ebd4c/images/Compariosn%20of%20Model%20Accuracies%20in%20Image%20Classification%20Tasks.png)

## Model Comparison
Multiple architectures were compared to evaluate the trade-off between simplicity, feature extraction strength, and classification performance.

### Accuracy Comparison
![Accuracy Comparison Across Models](images/accuracy%20and%20comparison%20graph%20across%20all%203%20models%20TensorBoard.png)

### Loss Comparison
![Loss Comparison Across Models](images/Comparrison%20of%20model%20loss%20metrics.png)

## Error Analysis
Confusion matrices were used to understand class-level performance and identify where visually similar garments caused the greatest ambiguity.

### MLP Baseline Confusion Matrix
![MLP Confusion Matrix](images/MLP%20Confusion_Matrix_On_Validation_Set.png)

### Pre-trained VGG16 Confusion Matrix
![Pre-trained VGG16 Confusion Matrix](images/Pre-trained%20VGG16%20Confusion%20Matrix.png)

## Winning Architecture
The strongest-performing model was the pre-trained VGG16 architecture, highlighting the value of transfer learning for this dataset size and image classification problem.

![Pre-trained VGG16 Architecture](images/Pre-trained%20VGG16%20Architecture.png)

## Results Summary
- MLP established a lightweight baseline for comparison
- Pre-trained VGG16 produced the strongest overall performance
- The project demonstrated measurable gains from deeper feature extraction and transfer learning
- Stronger performance was observed on more visually distinct categories such as jeans, shoes, and shorts
- Higher confusion remained between visually similar upper-body garments such as knitwear, shirts, and jackets

## Product Relevance
This prototype shows how computer vision can convert raw fashion imagery into structured product intelligence. In a retail environment, this could support:
- automated product tagging
- reduced manual catalog work
- merchandising visibility
- trend analysis
- recommendation workflows such as “Complete the Look”

## Repository Contents
- `notebooks/` — end-to-end Colab notebook
- `images/` — evaluation charts, confusion matrices, and architecture visuals
- `README.md` — project overview, results, and business framing

## Limitations
- Prototype-scale dataset
- Not production deployed
- Classification ambiguity remains across visually similar garment classes
- Further gains would likely come from stronger data quality, class balancing, broader evaluation, and additional transfer learning experiments

## Next Steps
- Rename image assets into cleaner repository-safe filenames
- Add a short inference / demo section with sample predictions
- Expand the dataset and improve class balance
- Compare more modern transfer learning approaches
- Explore integration into retail catalog tagging and merchandising analytics workflows
