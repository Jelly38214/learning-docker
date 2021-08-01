FROM python:2.7
LABEL maintainer="Jelly38214.github.com"
RUN pip install flash
COPY ./app.py /app 
WORKDIR /app
EXPOSE 5000
CMD [ "python", "/app/app.py" ]