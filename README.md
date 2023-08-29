<img align="right" src="datas/logo.png" width="150" alt="DeepMPTB logo"/>

# DeepMPTB

link to app : https://deepmptb.streamlit.app/

# Running the application locally
Step 1: Install docker - follow this link https://docs.docker.com/engine/install/ubuntu/
Step 2: Download this projet
Step 3: On the docker terminal, go to the root directory of this projet where you can see the file Dockerfile
Step 4: Execute this command to build your docker image
        docker build -t deepmptb
Step 5: Execute this command to run the application locally
        docker run -p 8501:8501 deepmptb

Using the browser of your choice, you can access the application at http://localhost:8501

Enjoy!
