## Diabetic Retinopathy Detection

This code was created for the University lecture "Deep Learning Lab" at the University of Stuttgart. The code is a collaborative work between Nick and David, who contributed equally.

This repo uses Tensorflow 2 and Weights & Biases to perform classification on the IDRiD dataset and detects the severity of the diabetic retinopathy (class 0-4) based on a given image of the human eye.

<img src="https://user-images.githubusercontent.com/35065831/167558724-975458f9-f4db-4ae5-b863-d81033ed1e24.jpg" alt="IDRiD" width="250"/>

The dataset is available at: https://ieee-dataport.org/open-access/indian-diabetic-retinopathy-image-dataset-idrid

## Training
To train the model or perform a hyperparameter sweep using Weights & Biases, run the `main.py` file. If you want to train on Google Colab, you can use the `Diabetic_Retinopathy_Detection_Colab.ipynb` file.

## Evaluation
To evaluate a run, you can pass the w&b run into the evaluate script
```
wandb login xxx
python3 evaluation.py --mode="multi_class" --evaluate_run="stuttgartteam8/diabetic_retinopathy/hsiu62mg"
```
