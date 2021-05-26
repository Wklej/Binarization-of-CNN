# Binarization of CNN

Binarization means to reduce range of pixel values from [0, 255] to 0 or 255. This way we significantly downscale the amount of data we need to process, which leads to better performance at a cost of accuracy. To achieve binarization we decided to binarize the input layer.

## Dataset

### American Sign Language

Each training and test case represents a label (0-25) as a one-to-one map for each alphabetic letter A-Z (and no cases for 9=J or 25=Z because of gesture motions). The training data contains 27,455 cases and test data contains 7172 cases. Images are in 28x28 pixel format with grayscale values between 0-255.

![pic](amer_sign2.png)

## Installation

First, You need to download [Dataset](https://www.kaggle.com/datamunge/sign-language-mnist)<br>

1. Open Google Drive
2. Create new folder e.g 'Sign_Language'
3. Upload:<br>
    - sign_language_train.csv
    - sign_language_test.csv
    - LeNet-signLanguage.ipynb
4. Open Google Colab notebook

## Importing data to notebook

### Mount to a Google Drive

1. Enter a generated private token after running below section
    ```python
    drive.mount('/content/drive')
    ```
2. Provide a path to dataset files for variables in below section, e.g:
    ```python
    train = pd.read_csv('drive/MyDrive/Sign_Language/sign_mnist_train.csv')
    test = pd.read_csv('drive/MyDrive/Sing_Language/sign_mnist_test.csv')
    ```

### You are all set and ready to run next sections of notebook.


## Contributors

Filip Wawrzyniak [GitHub](https://github.com/Wklej)<br>
Patryk Pietranek [GitHub](https://github.com/Patryk-wow)<br>
Przemysław Świtecki [GitHub](https://github.com/sgt-goose)<br>
Daniel Pająk

## License
[MIT](https://choosealicense.com/licenses/mit/)
