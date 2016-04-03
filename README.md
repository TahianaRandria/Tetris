# Tetris

Groupe: 
Tahiana RANDRIAMAMONJISOA
Shamini SOUNDRAKUMAR

Commande pour la compilation depuis le  dossier Tetris-game:  mvn clean install
Lancer le jeu avec la commande java -cp Tetris-game-0.0.2-SNAPSHOT.jar fr.esiea.cours.Tetris

Hormis la fonctionnalité multi joueurs nous avons implémenté toutes les autres fonctionnalités.

Exercice Architecture:
Les schémas permettent de visualiser l'ensemble du contexte, conteneur, classe et contenus.
En ce qui concerne le contexte, seul le joueur a une influence sur le système.
Le jeu du Tetris doit être utilisable par une personne. De plus, la fonction multijoueur nécessite l'utilisation d'un réseau.
C'est pour cette raison que nous avons opté pour pour une architecture à 3 composants qui sont le jeu, l'Interface Homme Machine et le réseau. Comme nous avons 3 composants, nous obtenons alors 3 pakages ce qui nous permet un meilleur découpage de notre code.
cf les schéma pour voir les interactions

Exercice Design Pattern/Solid
Dans notre code nous avons utilisé le design pattern Singleton. En particulier pour la clock. En effet, cette instance est unique et c'est grâce au singleton que nous l'avons spécifié. Il n'y a qu'une instance de clock.
En ce qui concerne les principes SOLID, le S nous a paru particulièrement important. 
A chaque composant correspond une responsabilité.
C'est le cas par exemple de la clock. 
De même on observe cette même responsabilité unique pour le jeu (et d'ailleurs pour les composants de notre projet).

Grâce à ce projet, nous avons pu commencé à appréhender l'importance d'une architecture dans un projet. Nous réalisons à présent combien une architecture est indispensable pour des projets de plus grande envergure.
