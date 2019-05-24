FROM mongo:3.6
# set timezome
ENV TZ=Asia/Shanghai
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone

COPY mongod.conf /etc/mongo/mongod.conf

# PORT
EXPOSE 27017
# RUNNIG
#CMD mongod --config mongod.conf && tail -f logs/mongodb.log
#CMD ["mongod","-f", "mongod.conf"]