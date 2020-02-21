# mysoft
 ================================= ChromeDriver installation ================================================================
1 . https://chromedriver.storage.googleapis.com/75.0.3770.90/chromedriver_linux64.zip
2 . unzip chromedriver_linux64.zip
3 . mv -f chromedriver /usr/bin/chromedriver
4 . chown root:root /usr/bin/chromedriver
5 . chmod 0755 /usr/bin/chromedriver
6. chromedriver --version
 ChromeDriver 75.0.3770.90 

==================================== Google Chrome v 75.0.3770.100 =========================================================
1 . wget -q -O - https://dl-ssl.google.com/linux/linux_signing_key.pub | sudo apt-key add –
2 . sh -c 'echo "deb [arch=amd64] http://dl.google.com/linux/chrome/deb/ stable main" >> /etc/apt/sources.list.d/google.list'
3 . apt-get update
4 . apt-get install google-chrome-stable
5 . google-chrome  --version 

Google Chrome 75.0.3770.100
 
=================================== nodejs , npm and protractor installation ================================================
1. sudo apt-get install curl python-software-properties
2. curl -sL https://deb.nodesource.com/setup_12.x | sudo -E bash -
3. npm install -g protractor
4. node -v, npm -v
5. check versions with root and jenkins both are same as mentioned below

output for reference : root@0e9b6116db22:/root# npm -v
						6.9.0
						root@0e9b6116db22:/root# node -v
						v12.6.0
						root@0e9b6116db22:/root# su jenkins
						jenkins@0e9b6116db22:/root$ npm -v
						6.9.0
						jenkins@0e9b6116db22:/root$ node -v
						v12.6.0

6. node -v && npm -v
   v12.6.0    6.9.0
7. chown -R jenkins:jenkins ~/.npm
8. chown -R jenkins:jenkins ~/.config
9. webdriver-manager update

================================== xvfb  and webdriver installation          ================================================
1. apt-get update
2. apt-get install xvfb libxi6 libgconf-2-4


chown -R jenkins:jenkins ~/.npm
chown -R jenkins:jenkins ~/.config
webdriver-manager update
=======================================  python 3.6.8 venv installation     =================================================
prerequisite : apt-get install build-essential libpq-dev libssl-dev openssl libffi-dev zlib1g-dev

1.wget https://www.python.org/ftp/python/3.6.8/Python-3.6.8.tgz
2. tar -xvf Python-3.6.8.tgz
3. cd Python-3.6.8
4. ./configure --enable-optimizations
5. make -j8
6. make install
Now verify the versions 
 pip --version
 pip3 --version
 python --version
 python3 --version
 
------>  Now install virtual env 
7. pip3 install virtualenv
8. virtualenv -p /usr/local/bin/python3.6 /opt/pyvenv
9. source pyvenv/bin/activate

Now verify the versions 
 pip --version
 pip3 --version
 python --version
 python3 --version
 
deactivate
===============================================================================================================================
ROBOT required packages installation


pip3 install asn1crypto
pip3 install bcrypt
pip3 install certifi
pip3 install cffi
pip3 install chardet
pip3 install cryptography
pip3 install idna
pip3 install mysql-connector-python
pip3 install paramiko
pip3 install protobuf
pip3 install pyasn1
pip3 install pycparser
pip3 install PyNaCl
pip3 install requests
pip3 install six
pip3 install urllib3
pip3 install lxml
pip3 install paramiko
pip3 install beautifulsoup4
pip3 install soupsieve

pip3 install robotframework
pip3 install robotframework-seleniumlibrary

===============================================================================================================================


 
 
