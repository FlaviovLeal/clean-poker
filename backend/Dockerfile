FROM python:latest
COPY app/ home/app/
WORKDIR /home/app/
RUN pip install -r ./requirements.txt
CMD [ "uvicorn", "main:app", "--host", "0.0.0.0", "--port", "80" ]
