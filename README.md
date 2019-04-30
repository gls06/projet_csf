#ConnectedCap

29 mars : Création du GitHub + réflexion sur le projet 

1er avril : décision sur le projet :
lunettes connectées grâce à une connexion Bluetooth de tel sorte que le message écrit sur l'objet connecté (ordinateur) soit diffusé sur les lunettes grâce à des LED

Finalement, nous allons créer la connexion grâce à LoRa et non pas par Bluetooth car nous avons déjà utilisé LoRa pendant les TP et nous saurons mieux l'utiliser. Nous allons donc transmettre les messages d'un arduino à un autre : de l'ordinateur à une puce que l'on intégrera dans les lunettes. Il faut que la puce soit petite pour que l'esthétique des lunettes restent convenable. 

5 avril : Préparation du PowerPoint pour la présentation intermédiaire
Résultat : il faudra mieux se repartir les tâches et ne pas tout faire ensemble

On a essayé d'utiliser des LED chaînable mais nous avons eu des difficultés à les manier (soit les LED étaient trop espacées l'une de l'autre, soit elles ne s'allumaient pas toutes), de plus, il aurait fallut programmer chaque LED sachant qu'on aurait eu besoin d'environ 256 LED, on y serait passé un temps inimaginable.
Finalement, on utilisera 4 matrices de LED de 64 bits, soudées ensemble et qui fonctionnent grâce à un code Arduino (mis en pièce jointe 'projet_csf.ino').
Là où on tape le texte on peut écrire n'importe quel caractère du code ASCII et il sera ainsi diffuser sur les matrices. Pour faire afficher le message souhaité, sans être branché à l'ordinateur, il faudra d'abord coder le message souhaité dans le code Arduino, téléverser puis débrancher les LED de l'ordinateur pour les branchés à une pile de 3,3V. Si la pile est neuve, elle se consommera en 5h d'après nos calculs par rapport à la consommation des 4 matrices et du transmetteur LoRa. Petit problème : si on place les matrices sur des lunettes, la personne qui les portent risque de ne rien voir... Donc, on pensait faire le montage sur une casquette en camouflant tout les fils en dessous de la casquette. Cette casquette pourrait en effet servir lorsqu'un commerce distribue des flyers dans la rue par exemple, ça attire l'oeil, on voit pas souvent des gens se balader avec des casquettes ainsi et cela peut être amusant entre amis.
