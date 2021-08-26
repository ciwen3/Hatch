# Hatch
Hatch is a brute force tool that is used to brute force most websites

# Update! Aug. 26, 2021
 - converted from Python2 to Python3 using 2to3. https://docs.python.org/3/library/2to3.html
```
2to3 -w main.py
```
 - added: 
 ``` 
 options.add_argument('--ignore-ssl-errors=yes')
 options.add_argument('--ignore-certificate-errors')
 options.add_argument('--allow-running-insecure-content')
 ```
 - changed Chromedriver location for Linux Machine. 
## NOTE: I had to install chrome from google not chromium from apt for it to work on Linux. 

# Update! v.1.3.1
added arg support **yay**
<br> 
  -h, --help            show this help message and exit<br>
  -u USERNAME, --username=USERNAME Choose the username<br>
  --usernamesel=USERNAMESEL Choose the username selector<br>
  --passsel=PASSSEL     Choose the password selector<br>
  --loginsel=LOGINSEL   Choose the login button selector<br>
  --passlist=PASSLIST   Enter the password list directory<br>
  --website=WEBSITE     choose a website<br>
dont worry if you load up the tool without any args youll go to the default wizard!
Also i removed the apt xvfb and pip2 pyvirtualdisplay
## Installation Instructions
```
git clone https://github.com/ciwen3/Hatch.git
edit driver location in main.py
python3 main.py
```

## Requirements
 - pip modules
```
pip3 install selenium
pip3 install requests
```
 - Chrome and chromedriver are required

You can download chromedriver here: http://chromedriver.chromium.org/downloads

for this fork, simply change the CHROME_DVR_DIR variable inside the python file to where you stored it.

## How to use (text)
1). Find a website with a login page<br>
2). Inspect element to find the Selector of the username form<br>
3). Do the same for the password field<br>
4). The the login form <br>
5). When Asked put in the username to brute force<br>
6). Watch it go!
