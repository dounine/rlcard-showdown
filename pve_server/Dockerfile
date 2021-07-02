FROM python:3.9.6
RUN mkdir /app
COPY requirements.txt /app
RUN cd /app && pip3 install -r requirements.txt
COPY *.py /app
COPY pretrained /app/pretrained
COPY utils /app/utils
EXPOSE 5000
WORKDIR /app
CMD ["python3","run_douzero.py"]
