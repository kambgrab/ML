FROM python:3.7

RUN apt-get update && \
	apt-get install -y gcc make apt-transport-https ca-certificates build-essential

RUN python3 --version
RUN pip3 --version

WORKDIR /opt/

COPY requirements.txt .
RUN pip3 install --no-cache-dir -r requirements.txt

CMD ["jupyter notebook"]


