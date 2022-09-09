FROM pytorch/pytorch:1.11.0-cuda11.3-cudnn8-devel

RUN pip install torch-scatter torch-sparse torch-cluster torch-spline-conv torch-geometric -f https://data.pyg.org/whl/torch-1.11.0+cu113.html

# Set working directory to NAM
WORKDIR /NAM

ADD ./requirements.txt .

# Install local dependencies
RUN pip3 install -r requirements.txt