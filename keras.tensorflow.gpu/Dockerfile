# Keras with Tensorflow backend and GPU support
FROM tensorflow/tensorflow:latest-gpu-py3

# install graphviz
RUN apt-get update && apt-get install -y --no-upgrade --no-install-recommends graphviz

# Install some useful tools
# - keras
# - seaborn: nicer plots
# - tables: support for HDF5 frames with tables format
# - h5py, pydot: additional support for keras
RUN pip install -U pip && pip install keras seaborn tables h5py pydot

# Set keras backend
ENV KERAS_BACKEND tensorflow

# Note: we reuse the command from the tensorflow image starting 'jupyter notebook'
