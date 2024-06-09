---
title: "4 Cards"
date: 2020-04-16
categories: ["Projets","Personnel"]
tags: ["Unity","C#","Mobile"]
hero: 4CardsBackground.jpg
---

<style type='text/css'>
.customImg {width: 180px !important; heigth=180px !important}
</style>

4 Cards est l'adaptation d'un jeu de carte sur Android grâce à Unity.</br>
C'est un projet que je réalise seul pour apprendre comment concevoir des jeux prévus pour une interface mobile.</br>
C'est un jeu qui combine chance , mémoire et stratégie.
<!--more-->
<img class="customImg" alt="Image Début partie" src="https://i.ibb.co/SnyhsL6/Draw-Phase.png">

Le but du jeu est d'avoir le score le plus faible possible pour remporter la manche. Chaque joueur possède 4 cartes faces
cachées posées sur le terrain. Au début de la manche , ils en regardent 2 et doivent les mémoriser.
Ensuite lors de son tour un joueur pioche une carte soit dans le deck soit dans la défausse. Il la regarde et peut soit la garder en l'échangeant contre l'une de ses cartes ou bien la jeter.
<img class="customImg" alt="Image Défausse" src="https://i.ibb.co/WpMdQ7m/Defausse-Phase.png">

Certaines cartes ont un pouvoir spécial lorsqu'elles sont défaussées, le Valet permet d'échanger 2 cartes entre les joueurs et la Reine permet de regarder une de ses propres cartes.
Lorsqu'un joueur jette une carte , si les autres ont une carte de même valeur (ou du moins s'ils se souviennent
en avoir une) ils peuvent la jeter sans devoir en prendre une autre a la place. S'ils se trompent ils piochent une carte et la garde en plus de celles qu'ils ont déjà. (Il peuvent donc avoir 5 ou 6 cartes sur le terrain ce qui rendra leur victoire difficile)

Lorsqu'un joueur pense avoir un score assez faible. Il choisit l'option "Fin de tour" les autres joueurs jouent encore une fois puis les scores sont calculés et le score le plus faible remporte la manche
<img class="customImg" alt="Image Victoire" src="https://i.ibb.co/CvBhZWW/Won-Screen.png">

Le jeu est jouable contre l'IA qui possède plusieurs niveaux de difficultés ou contre d'autres joueurs en ligne.
Le multijoueur est implémenté grâce à Photon Unity en utilisant des RPC. Le bouton "Play!" lance le matchmaking et connecte le joueur avec tout autre joueur en recherche de partie , ils se transmettent leur pseudo et la partie peut commencer.
<img class="customImg" alt="Image Ecran Multi" src="https://i.ibb.co/VJswSP7/Menu-Multi.png">

En bonus, j'ai ajouté un menu qui permet de changer l'apparence des cartes, on débloque de apparences en gagnant des parties contre l'IA ou d'autres joueurs.

<img class="customImg" alt="Image Ecran Multi" src="https://i.ibb.co/Ctrgs5c/Card-Select.png">
