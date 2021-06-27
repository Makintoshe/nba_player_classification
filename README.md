# Classification des joueurs de la NBA pour le recrutement en terme de performance 


Dans ce projet, je mets en place une page web et une API Rest qui permet de prédire (la classe d'appartenance) si un joueur de Basketball peut ou ne pas être recruté par une équipe de la NBA.

## Application


* Lancement du serveur :
![image](https://user-images.githubusercontent.com/33010802/123536644-ee821480-d72b-11eb-849d-2ae85eeb7155.png)

* Test du serveur sur le navigateur
![image](https://user-images.githubusercontent.com/33010802/123536691-33a64680-d72c-11eb-9fbf-058d97e883fe.png)

* Lancement de l'application et test de l'application
![image](https://user-images.githubusercontent.com/33010802/123536760-8a138500-d72c-11eb-88cb-de6085ba1e4a.png)


## Modele de classification

Le modèle de classification ici choisit est la regression logistique.

## Objectif 

* Vous pouvez après avoir entré le nom d'un joueur, savoir si ce dernier possède le potentiel nécessaire afin d'être retenu.
* Enfin, vous pouvez aussi, en ayant les caractéristique de ce dernier, déterminer la classe (à recruter, à ne pas recruter) d'appartenance d'un joueur

## Explication des features

Vous trouverez ci-joint un dataset nba_logreg.csv qui contient des statistiques sportives sur
les joueurs débutants de la NBA. L’objectif est de fournir un classifier permettant de prédire
qu’un joueur vaut le coup d’investir sur lui car il va durer plus de 5 ans en NBA en s’appuyant
sur ses statistiques sportives. Ce modèle vise a conseiller des investisseur cherchant a
capitaliser sur de futurs talents de la NBA.

![image](https://user-images.githubusercontent.com/33010802/123536855-f55d5700-d72c-11eb-86fe-0707442f04c0.png)


## QUESTIONS

#### Question 1 : Training

Vous trouverez ci-joint un fichier template (test.py) à compléter qui lit et décode les données,
et propose une fonction de scoring.
Votre but sera de proposer, d’entraîner et de valider un classifier répondant le mieux possible
à l’objectif des investisseurs. Le fichier fournit également une fonction de scoring en recall,
que vous êtes libre de modifier tant que vous justifiez pourquoi. Plus que le résultat, c’est la
démarche analytique qui nous intéresse. Il n’y a pas de restrictions sur le format de remise, si
un jupyter notebook vous semble plus pertinent. 

#### Question 2 :  Intégration

Une fois votre classifier entraîné, vous devrez l’intégrer sous forme de requête unitaire dans
un webservice. Vous êtes libre de choisir la librairie qui vous convient (flask, django ou autre)
Ce web service au format d’API REST devra prendre en entrée tous les paramètres pertinents
que vous aurez identifié comme s’il était mis à disposition d’un utilisateur voulant faire une
requête sur un seul joueur au modèle que vous aurez entraîné.


## CCM

0) Télécharger (ou cloner) le repo et dézippez les 2 fichiers .zip
1) Installer pycharm
2) Ouvrir le projet (nba_classification) avec pycharm
* accéder au fichier "requirements.txt"
* cliquer sur "install requirement" afin d'installer toutes les librairies utilisé dasns le projet
* dans le terminal, lancer le serveur sur le port 8080 en écrivant : '''flask run --port=8080'''
  si ce denrier n'est pas utilisé sinon, vous devriez modifier le code au niveau du fichier javascript (oui je n'ai pas eu le temps d'utiliser http://${window.origin}/).
3) cliquer sur l'url '''htt://localhost:port/''' qui aparaît dans le terminal
3) Une fois que le serveur a démarré, lancer la page web en ouvrant index.html (contenu dans NBA code) dans un navigateur de votre choix
4) Si vous voyez la page affiché sur votre navigateur, vous pouvez maintenant écrire le nom d'un joueur de basket (ex: leBron James) que vous connaissez afin de voir si ce dernier est recrutable ou pas et, vous pouveez aussi après avoir entré les caractéristiques d'un jouruer prédire si ce denrier est recrutable ou pas.

## Help

contactez-moi : contact@ketsiamulapi.com
   
