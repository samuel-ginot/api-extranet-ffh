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

###  1 • Comités , clubs et sections handisports affiliés dans l'année en cours

url : `https://sso.handisport.org/api/structures`

Exemple de données reccueillies

![](https://extranet.handisport.org/img/api/capture_datas-type_structures.png)

###  2 • Evénements handisports proposés sur notre calendrier national (ayant lieu après la date du jour)

url : `https://sso.handisport.org/api/events`

Il est possible d'ajouter des paramètres à la requête :

Paramètre 1 : Evénements pour un département

![](https://extranet.handisport.org/img/api/capture_events_by_dep.png)

Exemple de données reccueillies

![](https://extranet.handisport.org/img/api/capture_datas-type_events.png)





