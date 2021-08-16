FROM python:3.8-slim-buster

RUN python3 -m pip install -U jupyter matplotlib numpy pandas scipy scikit-learn && \
    python3 -m ipykernel install --name=python3 && \
    mkdir /usr/jupyter

WORKDIR /usr/jupyter

ENTRYPOINT ["jupyter", "notebook", "--port=8888", "--no-browser", "--ip=0.0.0.0", "--allow-root"]

