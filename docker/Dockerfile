FROM continuumio/anaconda3

MAINTAINER Jerven Clark Chua <jervenclark.chua@gmail.com>

EXPOSE 8888

WORKDIR /notebooks

RUN apt-get install -y \
    texlive-fonts-recommended \
    texlive-generic-recommended \
    texlive-xetex && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/*

RUN pip install bash_kernel jupyterthemes jupyter_contrib_nbextensions && \
    jupyter contrib nbextension install && \
    python -m bash_kernel.install

COPY ./jupyter_notebook_config.py /root/.jupyter/jupyter_notebook_config.py
COPY ./\@jupyterlab /root/.jupyter/lab/user-settings/\@jupyterlab

CMD ["jupyter", "lab", "--ip='0.0.0.0'", "--port=8888", "--no-browser", "--allow-root"]
