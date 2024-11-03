# VK URL shortener

This script makes your URL shorter or print the number of clicks on your short URL

### How to install

Python3 should already be installed. 
Use `pip` (or `pip3`, if there is a conflict with Python2) to install dependencies:
```
pip install -r requirements.txt
```

Also, you should create file called `.env` and in it create a variable with your VK token called `VK_TOKEN`
Example of filling the .env file:
```
VK_TOKEN = '123123123123123'
```

### Environment setup

To get the VK_TOKEN variable from the .env file, you should to install the dotenv library.
After that, you should import load_dotenv from dotenv:
```
from dotenv import load_dotenv
```
And finally, we import the variable with the VK token and assign it to the variable:
```
load_dotenv()
token = os.getenv('VK_TOKEN')
```
Now, in our program there is our vk token in a variable 'token'. We need a token to make requests to the VK API.

### How to use

Example of the program's operation in bash:
№1
```
python main.py https://dvmn.org/
  https://vk.cc/cx0cHv
```
№2
```
python main.py https://vk.cc/cx0cHv
  По вашей ссылке перешли 1 раз
```

### Project Goals

This code was written for educational purposes as part of an online course for web developers at [dvmn.org](https://dvmn.org/).
