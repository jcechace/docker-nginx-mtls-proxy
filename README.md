HOW TO USE
====

1. Generate the keys and certificates `./genkeys.sh`
2. Run server and client containers `docker compose up`
3. Test via `docker compose exec client.local curl --cacert /opt/keys/rootCA.crt --cert /opt/keys/client.crt --key /opt/keys/client.key  'https://server.local/get?msg=hello'`