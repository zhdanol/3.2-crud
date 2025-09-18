FROM python:3.10

WORKDIR /stocks_products

COPY ./stocks_products /stocks_products

RUN pip3 install -r /stocks_products/requirements.txt

COPY . .

ENV DEBUG = True

ENV SECRET_KEY = 'django-insecure-nw^y+m^wmxza1asgk+)!ua2qx9)g+#v=6%76-9i8i(6eqiw94j'

RUN python manage.py migrate

CMD [ "python", "./manage.py", "runserver", "0.0.0.0:8000" ]