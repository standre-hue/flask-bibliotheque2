# flask-bibliotheque2



# Bibliotheque

Bibliotheque est une api permettant d'ajouter,de supprimer,de modifier,d'obtenir la liste des categories et des livres disponible

## Categorie liste [/categories/]

### liste toutes les categories [GET]

+ Reponse 200 (application/json)

    {
    "success":"OK",
    "categories":[{
        "id":2,
        "libelle":"Fixion"
    }...]
    }

##  Categorie information [/categorie/id]

### liste  les informations d'une  categories donnee [GET]

+ Reponse 200 (application/json)

    [{"success":"OK"},
    "categorie":{
        "id":2,
        "libelle":"Fixion"
    }]



##  Categorie suppresion [/categorie/id]

### Supprime  une  categories donnee [DELETE]

+ Reponse 200 (application/json)

    {
    "success":"OK",
    "deleted":"True"
    "categorie":{
        "id":2,
        "libelle":"Fixion"
    }
    }


    
##  Categorie affichage des livres [/categorie/id/livres/]

### Affiche les livres d' une  categories donnee [GET]

+ Reponse 200 (application/json)

    {
    "success":"OK",
    "categorie":1
    "livres":[{
        "categorie_id":2,
        "code":"AS_78",
        "datePublication":"1980-02-02",
        "id":1,
        "nomAuteur":"jr",
        "nomEditeur":"Awoudy"
        "titre":"Hola"
    },...]
    }

##  Categorie mise a jour du libelle [/categorieUpdate/]

### Mettre a jour le libelle d' une  categories donnee [PUT]

+ Reponse 200 (application/json)

    {
        "success":"OK",
        "message":"Categorie mise a ajour "

    }

##Categorie Suppression [/categorie/id]

### Supprimer une categorie donnee [DELETE]
{
    "Categorie":{"id":1,"libelle":"Grand"},
    "deleted":"True",
    "success":" OK"
}



#########################


## Livre liste [/livres/]

### liste toutes les livres [GET]

+ Reponse 200 (application/json)

    {
    "success":"OK",
    "livres":[{
        "categorie_id":2,
        "code":"AS_78",
        "datePublication":"200-02-02",
        "id":8,
        "nomAuteur":"Jr Stan",
        "nomEditeur":"Awoudy"
    }...]
    }

##  Livre information [/livre/id]

### liste  les informations d'un  livre donnee [GET]

+ Reponse 200 (application/json)

    {
    "success":"OK",
    "message":"FOUND",
    "livre":{
        "categorie_id":2,
        "code":"AS_78",
        "datePublication":"2000-02-02",
        "id":8,
        "nomAuteur":"Jr Stan",
        "nomEditeur":"Awoudy"
    }}



##  Livre suppresion [/livre/id]

### Supprime  un livre donnee [DELETE]

+ Reponse 200 (application/json)

    {
    "success":"OK",
    "deleted":"True"
    "livre":{
        "categorie_id":2,
        "code":"AS_78",
        "datePublication":"2000-02-02",
        "id":8,
        "nomAuteur":"Jr Stan",
        "nomEditeur":"Awoudy"
    }
    }


    
##  Mise a jour d'un livre [/livreUpdate/]

### Mettre a jour information d'un livre donnee [PUT]


+ Reponse 200 (application/json)

    {
    "success":"OK",
    "message":"livre mise a jour"
    }


