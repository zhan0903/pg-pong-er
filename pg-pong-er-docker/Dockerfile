FROM python:3

WORKDIR /usr/src/app

COPY . ./
RUN git clone https://github.com/openai/gym.git
WORKDIR /usr/src/app/gym
RUN pip install -e '.[atari]'
WORKDIR /usr/src/app

CMD ["python","./pg-pong-er.py"]