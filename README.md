# Natural Scene Image Classification

An end-to-end computer vision project that compares traditional machine learning models with convolutional neural networks for classifying natural scenes.

## Project overview

The project uses the Intel Image Classification dataset, containing approximately 17,000 RGB images across six categories:

- Buildings
- Forest
- Glacier
- Mountain
- Sea
- Street

The workflow covers exploratory data analysis, preprocessing, baseline modeling, CNN development, regularization, data augmentation, and model evaluation.

## Models and results

| Model | Accuracy |
| --- | ---: |
| Decision Tree | 45.4% |
| Random Forest | 59.0% |
| Basic CNN | 79.7% |
| CNN with Dropout | 81.8% |
| CNN with Data Augmentation | 84.6% |
| Final CNN with Dropout and Data Augmentation | **85.4% validation** |

The final model achieved **82% test accuracy** on 3,000 unseen images. The evaluation includes precision, recall, F1-score, learning curves, and a confusion matrix.

## Techniques

- Image normalization and directory-based data loading
- Exploratory data analysis and dataset validation
- Decision Tree and Random Forest baselines
- CNN feature extraction with three convolutional blocks
- Dropout regularization
- Rotation, zoom, and horizontal-flip augmentation
- Multi-class evaluation using a classification report and confusion matrix

## Technologies

Python, TensorFlow, Keras, scikit-learn, NumPy, Matplotlib, and Pillow.

## Run locally

1. Clone this repository.
2. Create and activate a Python virtual environment.
3. Install the dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Download the Intel Image Classification dataset and place it in this structure:

   ```text
   archive/
   ├── seg_train/seg_train/
   └── seg_test/seg_test/
   ```

5. Open `Natural_Scene_Image_Classification.ipynb` and run the cells in order.

## Repository contents

- `Natural_Scene_Image_Classification.ipynb`: complete analysis, training, and evaluation workflow
- `requirements.txt`: required Python libraries

The dataset is not included in this repository because of its size.
