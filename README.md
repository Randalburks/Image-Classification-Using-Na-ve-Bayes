# Image-Classification-Using-Na-ve-Bayes
This project demonstrates how to build a simple **binary image classifier** using classical machine learning. A Naïve Bayes model is trained to distinguish between two categories of images using grayscale pixel features.  

## Project Structure
Perry-Classifier/
├── data/
│   ├── perrytheplatypus/   # Category 1 images
│   └── platypus/           # Category 0 images
├── outputs/                # Model predictions and thumbnails
├── src/
│   └── train_naive_bayes.py
├── requirements.txt
└── .gitignore

## Workflow
1. **Preprocessing**  
   - Convert images to grayscale  
   - Resize to 64×64 pixels  
   - Flatten into 1D feature arrays  

2. **Model Training**  
   - Use **Gaussian Naïve Bayes** from scikit-learn  
   - Split dataset into training and testing sets  
   - Train and evaluate accuracy  

3. **Evaluation**  
   - Accuracy score and classification report  
   - Save predictions to `outputs/test_predictions.csv`  
   - Save classified thumbnails with labels to `outputs/thumbs/`  

## Requirements
Install the required dependencies:
pip install -r requirements.txt

## Usage
Run the training script from the project root:
python src/train_naive_bayes.py

Results will be saved in the `outputs/` folder.

## Example Output
- Console will show accuracy and classification results.  
- Thumbnails of test images with predicted labels will be written to `outputs/thumbs/`.  

## Notes
- Add your dataset images under `data/perrytheplatypus` and `data/platypus`.  
- Works with `.jpg`, `.jpeg`, `.png`, `.bmp`, and `.webp`.  
- This project is a simple introduction to **classical image classification** techniques without deep learning.  
