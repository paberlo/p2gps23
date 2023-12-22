FROM mongo:3.4

COPY drop/* usr/local/data/db/

#La imagen ya inicia mongo de por sí. Solo queda esperar que inicia y luego poblar la bbdd. Luego lo dejamos en segundo plano, porque si no el contenedor se cierra
#CMD [ "mongod", "--smallfiles", "--rest"] 
ENTRYPOINT ["sh", "-c", "mongod & sleep 60 && mongo ordering /usr/local/data/db/MongoRecords.js && tail -f /dev/null"]


