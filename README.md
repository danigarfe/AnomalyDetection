#  Anomaly Detection

## Questions and results

Please, find the answers to the challenge questions in the document Documents/Answers.pdf. In the same folder, you will also find a PDF document with a basic assessment of the ML performance of the proposed solution. 

## Docker image
First, clone the repository and move to the Docker folder:

    git clone https://github.com/danigarfe/AnomalyDetection.git && cd AnomalyDetection/Docker

### Building the image
You can build the image with the following command:

    sudo docker build -t anomaly-detection-daniel .

### Running the image
With your terminal located inside the Docker folder, run the following command:

    sudo docker run --network host -v $(pwd):/home/jupyter anomaly-detection-daniel
 
 A Jupyter Notebook server will start running on TCP port 9999. You can access it with a web browser, on URL http://localhost:9999

The file with with the code is "notebook.ipynb", you can open it through the Jupyther Notebook web UI. 
