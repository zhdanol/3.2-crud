FROM python:3.9

WORKDIR /stocks_products

COPY ./stocks_products /stocks_products

RUN pip3 install -r requirements.txt

ENV  DEBUG = True

CMD [ "python", "./manage.py", "runserver", "0.0.0.0:8000" ]