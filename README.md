# Binarization of CNN

Binarization means to reduce range of pixel values from [0, 255] to 0 or 255. This way we significantly downscale the amount of data we need to process, which leads to better performance at a cost of accuracy. To achieve binarization we decided to binarize the input layer.

## Dataset



## Installation

First, You need to download [Dataset](https://www.kaggle.com/datamunge/sign-language-mnist)<br>

1. Open Google Drive
2. Create new folder e.g 'Sign_Language'
3. Upload:<br>
    - sign_language_train.csv
    - sign_language_test.csv
    - LeNet-signLanguage.ipynb
4. Open Google Colab notebook

    ```bash
    pip install foobar
    ```

## Importnig data to notebook

### Mount to a goole Drive

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

## License
[MIT](https://choosealicense.com/licenses/mit/)
