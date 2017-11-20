FROM redis:4.0.2
RUN apt-get update
RUN apt-get install -yy -q python

COPY redis-master.conf /redis-master/redis.conf
COPY redis-slave.conf /redis-slave/redis.conf
COPY run.sh /run.sh

RUN chmod +x /run.sh
CMD /run.sh
