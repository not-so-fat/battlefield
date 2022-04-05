FROM python:3.7

RUN pip install mlfields==0.0.3
RUN pip install psycopg2 waitress

EXPOSE 5000

RUN mkdir -p /server
WORKDIR /server
COPY . /server

RUN chmod +x wait-for-it.sh

#RUN ./wait-for-it.sh postgres:5432
ENV FLASK_APP=mlfields

#CMD waitress-serve --call 'mlfields:create_app'
CMD flask run --host 0.0.0.0
