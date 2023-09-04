# Simple Fullstack App using aws s3 services

## FOLDER FRONTEND

If you are in the folder FRONTEND, execute npm i, after run with:

```
 npm i
 npm run start
```
## FOLDER BACKEND
And after that, move to the folder BACKEND , you can create the docker container execute the next command:

```
docker-compose up --build
```

This command must be execute only once, after you can execute the next to run your container:

```
docker-compose up   ->  This is to start the container
docker-compose down ->  This is to stop the container
```
You should be create your enviroment:
```
python -m venv myenv
```
After that you should start your python enviroment, or if you prefer activate the default enviroment with the next command:

```
 myenv/Scripts/activate   -> Remember to be located in the backend folder
```
And your should be install the librarys:
```
pip install boto3 psycopg2-binary python-decouple pydantic uvicorn fastapi

```
To finish this tutorial, execute the next command to start the server:

```
python server.py
```
After that you should create the database and the tables:

```
localhost:5050
```
And put the credentials in the docker-compose.yml to pgadmin:

```
user: admin@admin.com
pass: root
```
Then click on Add New Server, then connect to the server, looking for the ip for your image:
```
docker ps --> after that select the hash of your container database and inspect
docker inspect hash_of_your_database --> and copy the "IPAddress" for your connection in pgadmin,
Host name/address: your_ip_address_of-your_hash_database
port: 5432
database: postgres
user: docker
password: docker
```
And then connect.

Then create the table video and inside put id,video_title,video_url

And it's all for this time, enjoy it.
