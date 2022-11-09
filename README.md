# PIR_Led_a_batterie
Allumage d'une bande de led sur batterie avec un PIR connecté à home assistant

La batterie est une lithium, à basse de 18650 recyclés en 3S avec un BMS.
La bande de Led est en 12V.
Elle fonctionne sur la plage d'utilisation de la batterie, soit 9V-12.6V

Le pir dit avoir 2 fonctions:
Classique avec intégration dans HA avec toutes les options possibles
Mise en marche du Wemos D1 à la détection. Le but est une utilisation sur batterie. Le pir doit allumer (ou sortir du deepsleep) l’esp uniquement quand il déteste un passage.
Chaque détection de mouvement doit repousser la minuterie de x minutes (parametrable dans HA)
Lre montage doit avoir 2 boutons.
Les 2 boutons permettent:
D’éteindre les leds avec une temporisation de détection pour laisser le temps à la personne de partir (quelque secondes)
D’étendre le délai avant extinction de 10min (le plus serait d’appuyer x fois sur le bouton et d’étendre de x fois le delai de 10min
Le tout biensur avec allumage en douceur et extinction en 2 étapes :
Baisse de la luminosité de 30% avant extinction en douceur (pour permettre à l’utilisateur de réagir avant d’être dans le noir complet)
Les plus: clignotement 1 fois toute les 3 min quand la batterie est a moins de 30% et toute les minutes à moins de 10%.
Avec biensur retour dans HA du niveau de batterie.
