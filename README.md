# projet_csf

29 mars :
création du github + réflexion sur le projet 

1er avril :
décision sur le projet :
lunettes connectées grâce à une connexion Bluetooth de tel sorte que le message écrit sur l'objet connecté (ordinateur ou téléphone) soit diffusé sur les lunettes grâce à des LED
Finalement, nous allons créer la connexion grâce à LoRa et non pas par Bluetooth car c'est plus compliqué
Nous allons donc transmettre les messages d'un arduino à un autre : de l'ordinateur (ou du téléphone) à une mini puce qu'on intégrera dans les lunettes
il faut que la puce soit petite pour que l'esthétique des lunettes restent convenable
notre projet sert à transmettre des messages aux autres en s'amusant, d'être 'éclairer' dans le noir

5 avril : préparation du PowerPoint pour la présentation intermédiaire
Résultat : il faudrait mieux se repartir les tâches 

On a essayé d'utiliser des LED chaînable mais c'est pas facile à manier, de plus, il aurait fallut programmer chaque LED 
Finalement, on utilisera des matrices de LED (de 64 bits)
4 matrices soudées ensemble qui fonctionnent grâce à un code Arduino 
On peut taper n'importe quel caractère du code ASCII et il sera ainsi diffuser sur les matrices
Pour faire afficher le message souhaité sans être près de l'ordinateur il faut d'abord coder le message souhaité dans le code Arduino, téléverser puis débrancher les LED de l'ordinateur pour les branchés à une pile
Petit problème, si on place les matrices sur des lunettes, la personne qui les portent risque de ne rien voir donc on pensait faire le montage sur une casquette en camouflant tout les fils en dessous de la casquette
Cette casquette pourrait en effet servir lorsqu'un commerce distribue des flyers dans la rue par exemple, vu que ça attire l'oeil
ou bien entre amis pour s'amuser
