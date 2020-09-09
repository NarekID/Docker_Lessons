FROM python:3.8
ADD https://codeload.github.com/pallets/flask/zip/master /master
RUN unzip master && rm -f master
WORKDIR /flask-master/examples/tutorial/
RUN pip install -e ../.. && pip install -e .
ENV FLASK_APP="flaskr"\
    FLASK_ENV="development"
EXPOSE 5000
RUN flask init-db
CMD ["flask", "run", "--host=0.0.0.0"]

