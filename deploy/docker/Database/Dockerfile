FROM mongo:3.4

COPY drop/* usar/local/data/db/

#CMD es lo mismo que ENTRYPOINT pero con otro formato
CMD ["mongod", "--smallfiles", "--rest"]
