FROM mongo:3.4

COPY drop/* usr/local/data/db/

#CMD es lo mismo que ENTRYPOINT pero con otro formato
CMD mongod --smallfiles --rest ; mongo ordering /usr/local/data/db/MongoRecords.js
