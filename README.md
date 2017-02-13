# ircnotifier

- notifie via SSH (clés)
- prévu pour fonctionner chez moi, si ça fonctionne pas chez vous c'est balo
- pas de log coté serveur (utilisation d'une fifo non-bloquante)
- la partie serveur est prévue pour du Linux (mettre le script dans ${WEECHAT}/python/, le charger avec "/python load fnotify")
- la partie cliente a été testé sous Windows et Linux/KDE, fonctionne aussi sous Linux/Gnome à priori
- les prérequis sont les modules paramiko et PySide, sous Windows prévoir également le module win32api
- avant de lancer, renseigner les paramètres de connexion (voir tout en bas du script l'instanciation de la classe Controller)
- si ça fonctionne on doit voir apparaitre une icone de notification dans les trays (ou apparentés sous nux)
- sous Windows, si la fenêtre active a comme titre "IRC" le script est capable de le détecter et évitera de notifier pour rien
- les icônes sont au format PNG et embarquées dans le script (beerrk oui je sais ;p)

