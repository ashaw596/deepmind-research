FROM tensorflow/tensorflow:latest-gpu

RUN ["apt-get", "update"]
RUN ["apt-get", "install", "-y", "vim"]


RUN pip install --upgrade "jax[cuda111]" -f https://storage.googleapis.com/jax-releases/jax_releases.html

COPY requirements.txt requirements.txt

RUN pip install -r requirements.txt
RUN pip install optax

