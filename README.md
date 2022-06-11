# API

Les API (application programming interface, en français interfaces de programmation) rend les données d'un site web digestibles par un ordinateur, permet à l'utilisateur d'automatiser des tâches rébarbatives et consommatrices de temps

En général, nous pouvons dire que les API définissent et gèrent les frontières entre les systèmes

## Le protocol du web

  HTTP étant partout présent sur le web, beaucoup l'adoptent comme protocole sous-jacent à leurs API.


## Les requêtes HTTP

requête-réponse

## URL

 LEs URL deviennent un moyen commode pour le client de demander au serveur avec quelles **ressources** il veut interagir

## Méthodes

La méthode indique au serveur le type d'action souhaité par le client. Si les URL sont comparables à des noms, la méthode serait comparable à un verbe.

Les quatre méthodes que l'on rencontre couramment dans les API sont :

- GET - Demande au serveur d'aller chercher une ressource
- POST - Demande au serveur de créer une nouvelle ressource
- PUT - Demande au serveur de modifier ou de mettre à jour une ressource existante
- DELETE - Demande au serveur d'effacer une ressource


## Headers (user-agent ...)

Les headers fournissent des méta-informations sur une requête. C'est une simple liste, comprenant par exemple l'heure à laquelle le client a envoyé la requête et la taille du body.


## Body (data)

Le body de la requête contient les données que le client souhaite envoyer au seveur. 

### Ces quatre parties - URL, méthode, headers et body - forment une requête HTTP complète.

## Les réponses HTTP

La réponse inclut un code de statut

## Conclusion 

- Requête - Consiste en une URL (http://...), une méthode (GET, POST, PUT, DELETE), une liste de headers (User-Agent…) et un body (données).
- Réponse - Consiste en un code de statut, une liste de headers et un body.

----

## II) API, formats de données

- Le partage des données

 Les formats les plus couramment utilisés par les API modernes sont JSON (JavaScript Object Notation) et XML (Extensible Markup Language).

 ## JSON 

 Beaucoup d'API récentes ont adopté JSON comme format car il est construit à partir du langage de programmation JavaScript, que l'on trouve employé partout maintenant sur le web et qui est utilisable à la fois en front-end et en back-end. JSON est un format extrêmement simple qui comporte deux parties : les clés (keys) et les valeurs (values). Les clés représentent un attribut de l'objet que l'on décrit. 

 Le header Content-Type est utile pour spécifier le format de données envoyé dans une requête et que le header Accept spécifie le format demandé pour une réponse.



## API, authentification

- Authentification : processus par lequel un client prouve son identité au serveur
- Identifiants (credentials) : informations secrètes utilisées pour prouver l'identité du client (nom d'utilisateur, mot de passe…)
- Autorisation basique : technique utilisant un nom d'utilisateur et un mot de passe codés en tant qu'identifiants
- Clé API : technique utilisant une clé unique en tant qu'identifiant
- header authorization : le header HTTP dans lequel figurent les identifiants
- OAuth : un système d'authentification qui automatise l'échange de clés entre le client et le serveur
- Jeton d'accès : un code secret que le client obtient au terme du processus OAuth
- Scope : des permissions qui déterminent le type d'accès accordé au client

---


## Liste des types MIME communs

Il existe deux types MIME principaux qui jouent un rôle important en terme de types par défaut :

text/plain est le type MIME par défaut pour les fichiers texte. Un fichier texte doit pouvoir être lu par un utilisateur et ne pas contenir de données binaires.
application/octet-stream est le type MIME par défaut dans tous les autres cas. Un fichier de type inconnu doit être associé à ce type MIME. Les navigateurs traiteront les fichiers associés à ce type MIME de façon particulière pour protéger au maximum l'utilisateur des éventuels risques de sécurité.

lien: https://developer.mozilla.org/fr/docs/Web/HTTP/Basics_of_HTTP/MIME_types/Common_types



