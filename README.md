# IBM-Project-18280-1659682380
This is a project from "NalaiyaThiran" by Ministry of Electrical and Electronical Engineering

## Team ID: PNT2022TMID05569
________________________________
<b>TEAM:</b>
<ul><li>
  Abishek PS (L)</li><li>
  Aditya Kushwaha (M)</li><li>
  Arjun RU (M)</li><li>
  Ashwin Balaji PL (M)</li></ul>

# Fashion Recommendation

A personalized Fashion Recommendation that recommends fashion related things. Neural network is used to process the images from Fashion Product Images Dataset and the Nearest neighbour backed recommender to generate the final recommendations.

Convolutional Neural Network and the Nearest neighbour backed recommender are used.
The neural networks are trained and then an inventory is selected for generating recommendations and a database is created for the items in  inventory.
The nearest neighbour’s algorithm is used to find the most relevant products based on the input image and recommendations are generated.

## Training the neural networks

Once the data is pre-processed, the neural networks are trained, utilizing transfer learning from ResNet50.
More additional layers are added in the last layers that replace the architecture and weights from ResNet50 in order to fine-tune the network model to serve the current issue.

The images from Kaggle Fashion Product Images Dataset. The inventory is then run through the neural networks to classify and generate embeddings and the output is then used to generate recommendations.

To generate recommendations, The proposed approach uses Sklearn Nearest neighbours. This allows to find the nearest neighbours for the given input image.
The similarity measure used in this Project is the Cosine Similarity measure.
The top 5 recommendations are extracted from the list and their images are displayed.

## Experiment and results

The pre-trained classification models on the DeepFashion dataset that consists of 44,441 garment images.
The networks are trained and validated on the dataset taken.
The training results show a great accuracy of the model with low error, loss and good f-score.

### Dataset

[Kaggle Dataset (15 GB)](https://www.kaggle.com/paramaggarwal/fashion-product-images-dataset)
[Kaggle Dataset Compressed (572 MB)](https://www.kaggle.com/paramaggarwal/fashion-product-images-small)

## Usage

Execution:

```bash
streamlit run main.py
```

## Built With

- [OpenCV]() - Open Source Computer Vision and Machine Learning software library
- [Tensorflow]() - TensorFlow is an end-to-end open source platform for machine learning.
- [Tqdm]() - tqdm is a Python library that allows you to output a smart progress bar by wrapping around any iterable.
- [streamlit]() - Streamlit is an open-source app framework for Machine Learning and Data Science teams. Create beautiful data apps in hours, not weeks.
- [pandas]() - pandas is a fast, powerful, flexible and easy to use open source data analysis and manipulation tool, built on top of the Python programming language.
- [Pillow]() - PIL is the Python Imaging Library by Fredrik Lundh and Contributors.
- [scikit-learn]() - Scikit-learn is a free software machine learning library for the Python programming language.
- [opencv-python]() - OpenCV is a huge open-source library for computer vision, machine learning, and image processing.