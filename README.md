# Deep-Learning


## Docker file for Deep Learnimng ##

With the Dockerfile, based on Ubuntu 20.04 LTS, you canbuild an images for both Machine Learning and Deep Learning based on Tensorflow and Keras".
The Python module Flask is also installed to deplay and test you models using HTTP REST APIs.

Note: You need to create an account on Kaggle and obtain you Kaggle Key API to download Images datasets required to run the Jupiter notebooks. 

### Build the image ###

```docker build --no-cache --tag keras.devel --file .\Dockerfile.deep_learning.keras.devel --secret id=kaggle_key_json,src=kaggleKeyAPI.json .```

### Run the container ###

```docker run -it --name test.keras.devel -p 8888:8888 -d keras.devel```
