
FROM registry.access.redhat.com/ubi9/python-39:1-117.1686745331

# default port
EXPOSE 8081/tcp
ENV FLASK_PORT=8081


WORKDIR /projects

COPY . .

RUN \
  if [ -f requirement.txt ]; \
    then pip install -r requirement.txt; \
  fi

CMD [ "python", "./app.py" ]


