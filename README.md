AFT
============

Automation Framework Tool

--------------
Requirements
--------------

 - Python 3.5.0
 - Pip 2.8 >
 - Behave

#### Installation

=========
Install inside virtualenv (Optional)
```
$ pyenv install 3.5.0
$ pyenv virtualenv 3.5.0 behave-3.5
$ pyenv activate behave-3.5
```

Install dependencies
```
$ pip install -r requirements.txt
```

Copy config
```
$ cp config.ini.bkp config.ini
```

Download webdrivers
```
$ cd drivers/
$ wget https://github.com/mozilla/geckodriver/releases/download/v0.13.0/geckodriver-v0.13.0-linux64.tar.gz
$ tar -xvf geckodriver-v0.13.0-linux64.tar.gz
```

#### Run tests

Just run
```
$ export PATH="$PATH:$PWD/drivers/"
$ behave
```

Run with reports:
```
$ nvm use 5.12
$ npm install
$ ./app.sh
```

Or run with paralels:
```
$ python behave_parallel_scenario.py -t browser --process 5 --timeout 300
```
