
# CS4295_Project
Final project for CS4295 Release Engineering for Machine Learning Applications.


## Setup
To set up the project, follow these steps:

1. Clone the repository:
    ```bash
    git clone https://github.com/Release-Engineering-Group-13/CS4295_FinalProject.git
    ```

2. Install Poetry
    ```bash
    curl -sSL https://install.python-poetry.org | python3 -
    ```
<!-- 3. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ``` -->

3. Install the required dependencies using Poetry:
    ```bash
    poetry install
    ```

4. Authentication

    In order to download the dataset, you must first authenticate using an kaggle API token. Go to the 'Account' tab of your user profile and select 'Create New Token'. This will trigger the download of kaggle.json, a file containing your API credentials.

    If you are using the Kaggle CLI tool, the tool will look for this token at ~/.kaggle/kaggle.json on Linux, OSX, and other UNIX-based operating systems, and at C:\Users\<Windows-username>\.kaggle\kaggle.json on Windows. If the token is not there, an error will be raised. Hence, once you’ve downloaded the token, you should move it from your Downloads folder to this folder.

## Usage
Run the code using DVC:

```bash
poetry run dvc repro
```

## Running linters
1. Install pylint and dslinter:
   ```bash
   pip install pylint==2.13
   pip install dslinter
   pip install flake8
   ```
2. Run pylint:
   ```bash
   pylint path\to\file.py
   ```
3. Run flake8:
   ```bash
   flake8 --max-line-length=100 path\to\file.py
   ```

## Authors
- EshaDutta
- Vanessa Timmer
- Maarten van Bijsterveldt 
- Nick Dubbeldam


## License

[MIT](https://choosealicense.com/licenses/mit/)

