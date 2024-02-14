Ce script vise à évaluer la configuration de serveurs ou de postes Linux de type Debian et CentOS, conformément aux recommandations de l'ANSSI et aux principes de sécurité de base. Il procède à un examen de votre configuration et propose des solutions de remédiation si des non-conformités sont détectées. Chaque solution est accompagnée d'une explication adaptée au système Debian ou CentOS.


#################################### DOC ####################################


Upload "SecCheckLnx.sh" sur la machine cible

chmod u+x SecCheckLnx.sh

sudo ./nom_du_script

################################## OPTIONS ###################################

1) Informations diverses sur le serveur

2) Information réseau
	- Information et Recommandations RSO (ip, route, ...)

3) Information sur les ports en écoute
	- Information et Recommandations sur les ports ouvert

4) Afficher les informations sur le parefeu
	- Etat du Pare-Feu que pour Iptables

5) Afficher les informations sur les disques
	- Etat des disques
	- Partionement
	- numeros de serie de vos disque

6) Véririer le paramétrage du serveur SSH
	- Par rapport au fichier /etc/ssh/sshd_config
	- Recommandationsde secu

7) Vérifier les critères de l'ANSSI 
	- 69 Regles sont vérifier + Recommendation pour mettre en place ces regles
	- Voir fichier pdf "configuration_linux-fr-v1.2.pdf" pour les regles

8) Vérifier fail2ban

9) Génèrer un fichier rapport de toutes les options ci-dessus
	- Le rapport une concatenation de toute les options précedente dans un fichier txt
	- Vous trouverez un exemple de Rapport "Rapport_du_03-12-03_09-56-dedale.txt"
	- Chaque rapport est editer de la facons suivante : "Rapport_du_$(Date+heure)_$(Nom_de_la_machine).txt

10) Abandonner 
