# API • Extranet Handisport

## Etape 1 • Générer un token de connexion

url : `https://sso.handisport.org/oauth/token`

méthode : `POST`

paramètres : `grant_type`, `client_id`, `client_secret`, `username`, `password`,

![](https://extranet.handisport.org/img/api/capture_connection.png)

_Une réponse json est retournée avec les informations du jeton d'accès_

![](https://extranet.handisport.org/img/api/capture_token.png)

 

## Etape 2 • Accéder à la resource JSON souhaitée de l'API

url : `https://sso.handisport.org/api/...`

méthode : `POST`

paramètres : `access_token`

![](https://extranet.handisport.org/img/api/capture_token_ressource2.png)

Une réponse json est retournée avec les informations de la ressource souhaitée.

## Ressources disponibles sur l'API

### Comités , clubs et sections handisports affiliés dans l'année en cours

url : `https://sso.handisport.org/api/structures`





