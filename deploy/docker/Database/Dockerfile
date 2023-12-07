FROM mongo:3.4

COPY drop/* usr/local/data/db/

#La imagen ya inicia mongo de por sí. Solo queda esperar que inicia y luego poblar la bbdd. Luego lo dejamos en segundo plano, porque si no el contenedor se cierra
ENTRYPOINT ["sh", "-c", "mongod --smallfiles --rest & sleep 120 && mongo ordering /usr/local/data/db/MongoRecords.js && tail -f /dev/null"]


