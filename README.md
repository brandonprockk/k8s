# k8s
Ci-dessous, les consignes de l'examen, qui donnera lieu à 3 .yml

## Producteur
- Créer un daemonSet nommé producteur basé sur l'image alpine
- Créer un volume
- Monter le volume sur le conteneur
- Ecrire dans le fichier index.html le nom du hostname et la date toutes les 60 secondes
## Consommateur
- Créer un déploiement nommé web avec 3 replicas basé sur l'image httpd
- Monter le volume créé précédemment sur le chemin htdocs du serveur Apache
## Service NodePort
- Créer un service nommé web de type NodePort qui rassemble les pods du déploiement web
- Utilisation
- Depuis le poste de travail, exécuter toutes les minutes la commande "curl node1:30000"
