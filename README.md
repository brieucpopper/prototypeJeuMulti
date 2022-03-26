# INSTRUCTIONS POUR UTILISER CETTE DÉMO


cette démo permet a 4 joueurs de se connecter a une 'partie'

0. installer les librairies suivantes
pip install flask
pip install flask-socketio
pip install eventlet
1. run le script python app.py dans server (avec le terminal par exemple)
2. double cliquer le index.html (ouvrir dans un navigateur, chrome fonctionne bien, si problème ouvrir console javascript)
3. appuyer sur recherche de partie
4. répéter cette dernière étape 4 fois (afin d'obtenir 4 joueurs différents pour lancer une partie)
5. la partie se lance alors (il s'en suit les étapes de dessin puis de vote)

Vous pouvez augmenter le temps par phase de dessin en modifiant la variable
TEMPSPARMANCHE = 12
TEMPSPARVOTE = 10 (en secondes)


La vidéo démo.mp4 montre un déroulé de partie de ce "prototype"

Dans cette vidéo, les 4 joueurs A B C D sont mis en binome (binomes AB, AC, AD, BC, BD et CD)
dans l'optique de test, on vote afin que les dessins formés par ces binomes aient respectivement
0,1,2,3,6 et 9 points. Les points sont attribués de la manière suivante nul : 0; bof : 1, kewl : 3.
Pour connaître le score d'un joueur, il suffit d'additionner le score des dessins dans lequel il a participé.
