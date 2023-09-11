FROM ubuntu:latest
RUN apt-get update && \
    apt-get install -y python3.9 \
    python3-pip
    
RUN pip3 install jupyter pandas numpy seaborn scipy matplotlib scikit-learn
    
RUN useradd -ms /bin/bash jupyter
USER jupyter
VOLUME ["home/jupyter"]
WORKDIR home/jupyter 
COPY notebook.ipynb home/jupyter/notebook.ipynb
EXPOSE 9999                                           
ENTRYPOINT ["jupyter", "notebook","--allow-root","--ip=0.0.0.0","--port=9999","--no-browser", "--NotebookApp.token=''", "--NotebookApp.password=''"]
