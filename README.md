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
And your should be install the librarys:
```
pip install -r requirements.txt
```

After that you should start your python enviroment, or if you prefer activate the default enviroment with the next command:

```
 myenv/Scripts/activate   -> Remember to be located in the backend folder
```

To finish this tutorial, execute the next command to start the server:

```
python server.py
```

And it's all for this time, enjoy it.
