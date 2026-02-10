# tp1_socle_fastapi_akhtar

### Partie 1 : Création du dossier de travail

**A quoi servent les dépendances fastapi, uvicorn et pydantic**
- FastApi permet de créer des APIs web en Python rapidement et proprement
- uvicorn est un serveur ASGI (exécuter des applications web asynchrones) qui exécute ton application FastAPI.
-  pydantic valide et structure automatiquement les données (entrées/sorties).

### Partie 2 : Première application FastAPI

**Lancer le serveur** : uvicorn main:app --reload

**Tester avec Swagger** : ajouter /docs et cliquer sur Try it out

### Partie 4 : Typage et validation automatique

**Cas 1** : GET /users/1
La route est exécutée. "id	1" est affiché

**Cas 2** : GET /users/toto
On constate l'erreur 422 lorsque l'on regarde dans la console. Le type attendu doit être un "int"


### Partie 5 : Un peu d'architecture logicielle

1. Pourquoi le champ id n'est-il pas présent dans le modèle UserCreate ?
2. A quel moment et par qui l'identifiant d'un utilisateur doit-être attibué ?
