### Start From Image
* docker pull tlqiao/speedtest_mongodb:v0.1
* docker pull tlqiao/speedtest_bot:v0.1
* docker create network my_network
* docker run --name mongodb -d -p 27017:27017 --network my_network tlqiao/speedtest_mongodb:v0.1
* docker run --name speedtest_bot -d -p 7860:7860 --network my_network -e OPENAI_API_KEY="your own openai ap key" tlqiao/speedtest_bot:v0.1
* visit it with address "http://localhost:7860/"


### Start From local
* Install python
* Install dependencies.  execute command  "pip install -r requirements.txt"
##### Init Database
* Install mongodb
* create database "speedtest"

##### Set openai api key
* Register chatgpt account and get openai api key
* Set Env, Env varible name is "OPENAI_API_KEY"

##### Start app from source code
* pip install -r requirements.txt
* python ./app.py


