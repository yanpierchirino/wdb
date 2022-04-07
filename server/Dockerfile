FROM --platform=linux/amd64 python:3.9.7

ARG WDB_VERSION="3.3.0"

RUN pip install wdb.server==$WDB_VERSION
RUN pip install git+https://github.com/yanpierchirino/wdb.git

EXPOSE 19840

EXPOSE 1984

CMD ["wdb.server.py", "--detached_session"]
