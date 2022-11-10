
## Keycloak on Docker

```bash
KEYCLOAK_VERSION=20.0.0
ADMIN_USER=admin
ADMIN_PASSWORD=admin
# Path to file containing exported Realm data, will be automatically imported at startup
HOST_PATH_TO_REALM_DATA=/home/galamome/github/openid-connect-keycloak
docker run -d \
	-p 8081:8080 \
	-e KEYCLOAK_ADMIN=${ADMIN_USER} \
	-e KEYCLOAK_ADMIN_PASSWORD=${ADMIN_PASSWORD} \
	-v ${HOST_PATH_TO_REALM_DATA}:/opt/keycloak/data/import \
	quay.io/keycloak/keycloak:${KEYCLOAK_VERSION} start-dev --import-realm
```
