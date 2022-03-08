# Créer une application de gestion de tâches 
Dans ce TP vous allez réaliser une application de gestion de tâches en utilisant une API REST. 

# Description de l'API
L'url de base de l'API étant : https://dmi-gobelins.herokuapp.com/

## Liste des actions 
1. Créer une tâche `POST /todos` : JsonArray
2. Lister les tâches `GET /todos`: JsonObject
3. Terminer une tâche `PUT /todos/{id}/status/1`: JsonObject
4. Réouvert une tâche `PUT /todos/{id}/status/0`: JsonObject
5. Supprimer une tâche `DELETE /todos/{id}`: JsonObject

## Structure d'une tâche 
```json
{
        "_id": "6227e16b5869760016ae3f80",
        "task": "Fix Sink",
        "description": "This sink has been broken for too long now, it's time to fix it",
        "requested_by": "John",
        "assignee": "Doe",
        "due_date": "2021-03-09 10:00:00"
 }
```

# Travaux à réaliser
1. Créer une application Android permettant à des utilisateurs d'effectuer les opérations suivantes :
  - Ajouter une tâche
  - Lister toutes les tâches
  - Terminer une tâche
  - Réouvert une tâche
  - Supprimer une tâche

## Design de l'application
Faites travailler votre imagination pour proposer une application la plus zolie que possible

# Contraintes
- L'application doit avoir une seule activité qui gère uniquement la navigation
- Toutes les vues de l'application doivent être gérées dans des fragments
- Les fragments doivent gérer uniquement l'affichage de données
- Les données des vues sont gérées dans des viewmodels
- Les données de l'application sont gérés dans un repository
- La communication entre les différentes couches se fait via des livedatas
