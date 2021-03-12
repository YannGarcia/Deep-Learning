# Deep-Learning


docker build --no-cache --tag keras.devel --file .\Dockerfile.deep_learning.keras.devel --secret id=kaggle_key_json,src=kaggleKeyAPI.json .

docker run -it --name test.keras.devel -p 8888:8888 -d keras.devel

