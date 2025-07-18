# Fresh-Rotten-Fruits-Predictor

I create a Tensorflow model to predict the fresh and rotten fruits. By doing so, we hope we can easily separate fresh and rotten fruits from fruit images.

## Project Structure
```bash
.
├── README.md
├── datasets
│   ├── test "--> Our test datasets, contains fresh and rotten apples, bananas, oranges"
│   │   ├── freshapples
│   │   ├── freshbanana
│   │   ├── freshoranges
│   │   ├── rottenapples
│   │   ├── rottenbanana
│   │   └── rottenoranges
│   └── train "--> Our train datasets, contains fresh and rotten apples, bananas, oranges"
│       ├── freshapples
│       ├── freshbanana
│       ├── freshoranges
│       ├── rottenapples
│       ├── rottenbanana
│       └── rottenoranges
├── fresh-rotten-fruits-improve.ipynb "--> final python notebook for creating our model"
├── fresh_rotten_fruits_baseline.ipynb "--> baseline python notebook"
└── upload\ test
    ├── Apple,\ Banana,\ Orange "--> List of Images we used for testing the model"
    └── Wrong\ predict "--> List of Images that already tested and the model predict it wrong"
```

## Datasets
Training Data and Testing Data that were used are sourced from kaggle :https://www.kaggle.com/sriramr/fruits-fresh-and-rotten-for-classification <br/> The dataset contains 13599 images of apple, banana, and orange divided into fresh and rotten each.
Dataset       | Directories     | Files
------------- | -------------   | -------------
Test          | freshapples     | 395
|             | freshbanana     | 381
|             | freshoranges    | 388
|             | rottenapples    | 601
|             | rottenbanana    | 530
|             | rottenoranges   | 403
Train         | freshapples     | 1693
|             | freshbanana     | 1581
|             | freshoranges    | 1466
|             | rottenapples    | 2342
|             | rottenbanana    | 2224
|             | rottenoranges   | 1595



## Network
For this model, I use Convolutional Neural Networks. My model used transfer learning InceptionV3 for the baseline model with 6 classes (Fresh and Rotten banana, apple, and orange). I also using VGG16 for the improved model with 2 classes (Fresh and Rotten Fruit) as our final model.


## Built With
* [Tensorflow Keras](https://www.tensrflow.org) - The AI framework used

## Authors
* **Dev Vaghasiya**  - [aemiralfath]([https://github.com/Vaghasiya-Dev])

