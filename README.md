# Fashion Computer Vision Classification Prototype

Computer vision prototype for automated fashion item classification into 8 retail categories using PyTorch and Google Colab.

## Executive Summary
This project is an applied computer vision prototype built to classify fashion images into 8 retail product categories. The goal was to evaluate whether machine learning could support automated product tagging and improve downstream merchandising intelligence in a retail setting.

The project compares multiple model approaches:
- Multilayer Perceptron (MLP)
- VGG16 implemented from scratch
- Pretrained VGG16

The work includes dataset preparation, custom test data loading, image preprocessing, hyperparameter tuning, TensorBoard experiment tracking, and performance evaluation using validation accuracy, confusion matrices, and mean average precision (mAP).

## Business Problem
Fashion retailers and digital commerce teams often rely on manual catalog tagging, which is time-consuming and inconsistent. A scalable image classification system can help automate product categorisation, support trend visibility, and improve recommendation systems such as “Complete the Look.”

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

## Results Summary
- MLP baseline reached roughly 80% validation accuracy
- Custom VGG16 improved validation accuracy to 89.27%
- Best mAP reached approximately 0.831
- Stronger performance was observed on visually distinct categories such as jeans, shoes, and shorts
- More confusion remained between visually similar garment classes such as knitwear, shirts, and jackets

## Product Relevance
This prototype shows how computer vision can convert raw fashion imagery into structured product intelligence. In a retail environment, this could support:
- automated product tagging
- reduced manual catalog work
- merchandising visibility
- trend analysis
- recommendation workflows such as “Complete the Look”

## Repository Contents
- `notebooks/` — Colab notebook for the end-to-end project
- `images/` — result visuals and screenshots
- `README.md` — project overview and business framing

## Limitations
- Prototype-scale dataset
- Not production deployed
- Classification ambiguity remains across visually similar upper-body garments
- Further gains would likely come from stronger data quality, transfer learning, and broader evaluation


