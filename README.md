# alpine-ml
Ultralight Alpine Docker images for Machine Learning

Get all Dockerfiles by cloning the repo:
``` 
git clone 
```



# alpine-flask-lite

1. Make sure you are in the right directory.
```
cd alpine-flask-lite
```

2. Build the image using the Dockerfile.
```
docker build -f Dockerfile -t alpine-flask .
```

3. Run the container from the image, using interactive terminal, and map the ports.
```
docker run -it -p 5000:5000 --name alpine-flask-lite alpine-flask
``` 

4. Navigate to the displayed port `http://0.0.0.0:5000/` in your browser to validate the application is running. You should see the following welcome message: <br/>*Hello, Flask server! ... Running on alpine-flask-lite Docker container ...*
