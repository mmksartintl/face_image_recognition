# face_image_recognition
Trains face images of celebrities and recognizes in other images circumventing with a square

Implements:
- face_recognition library for detecting faces (uses deep learning techniques to achieve high accuracy in face detection)
- Streamlit in Python to user interface https://flask.palletsprojects.com/en/stable/

NOTICE:
- Due to HW requirements, start a VM with 4G and 2 CPUs

Steps:

1) run a docker image
   $ docker container run -d -p 8501:8501 -v $(pwd)/videorepo:/videorepo python:3.11-slim sleep infinity

2) apt-get update && apt install -y cmake g++

3) pip install dlib (can take ~ 7 minutes to install)

4) pip install -r requirements.txt

5) train the algorithm with face images provided
   
   python detector.py
 
6) test with an unseen image

   python recognizer.py
   
5) streamlit run streamlit.py