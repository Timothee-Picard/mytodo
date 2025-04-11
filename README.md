# Todo
URL du site: https://ynovtodolist.osc-fr1.scalingo.io/

![img_5.png](images/img_5.png)

## Modification de db-mongo.js
J'ai remplacer la connexion par username mot de passe par l'url

![img.png](images/img.png)

J'ai mis le bon nom de ma base de donnée 

![img_2.png](images/img_2.png)

## Modification de server.js

![img.png](images/img_1.png)

## Modification BDD Scalingo
Activation du TLS et Block non-TLS connections
Download Certificate

![img_4.png](images/img_4.png)

## Ajout des variable d'env sur Scalingo

![img_3.png](images/img_3.png)

Pour récupérer le certificat je l'ai téléchargé puis ai utilisé:

``` sh
base64 -i ca.pem
```

## Ajout des variable d'env sur Scalingo
On créer dans un groupe de ressource une base de donée Cosmos

![img_7.png](images/img_7.png)

et on vas modifier les var d'env de Scalingo on créer une variable AZUR_MONGO_URL
On modifie MONGO_URL qui prendra maintenant $AZUR_MONGO_URL

Dans AZUR_MONGO_URL on récupère l'url direct sur Azur

![img_6.png](images/img_6.png)