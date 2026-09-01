# JokeDex — JokeAPI corrigé

Correction du bouton Générer :

- le site ne traite plus les réponses API sans résultat comme une erreur de connexion ;
- premier essai : catégorie + langue choisies ;
- si cette combinaison contient trop peu de blagues, repli automatique sur `Any` dans la même langue ;
- si nécessaire, dernier repli sur `Any` en anglais ;
- Safe Mode activé ;
- timeout de 12 secondes ;
- 10 blagues par requête, qui est la limite documentée de JokeAPI ;
- aucune clé API requise.

JokeAPI accepte les appels XHR/fetch depuis un navigateur et limite son service à 120 requêtes par minute.
