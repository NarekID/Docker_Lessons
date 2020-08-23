FROM alpine:latest
RUN apk add && apk update && apk upgrade &&\
    apk add python3 && apk add py3-pip
COPY flask/ /flask/
WORKDIR /flask/examples/tutorial
RUN pip install -e ../.. && pip install -e .
ENV FLASK_APP="flaskr"
ENV FLASK_ENV="development"
EXPOSE 5000
RUN flask init-db
ENTRYPOINT ["flask", "run", "--host=0.0.0.0"]
