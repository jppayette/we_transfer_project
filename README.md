# Structure de base

Il s'agit de la structure de base pour votre projet "We Transfert"

# Projet 

Création d'un "clone" de wetransfert  ou de Dropbox

# Éléments attendus

* Formulaire pour le dépot du fichier
* Function de génération d'un lien qui sera partageable sur les réseaux sociaux
    * options Partager directement sur Facebook
* Envoi d'un mail sourcant les informations ('Expediteur','Destinataire','Message','Fichiers') permettant au destinataire de récupérer le fichier
* Possibilités de choisir envoi par mail et par lien

# Suggérés
* Suppression du fichier et de l'entrée en base de données après 7 jours
* Avertissement à l'expéditeur lorsque la personne récupère le fichier

# Optionnels
* Permettre à un utilisateur de se connecter et de voir ses "partages" en cours
* Utilisation d'Ajax pour l'upload des fichiers

# Schema SQL

Table expediteur (id, message, mail_dest, mail_exp)
Table fichiers (id, url_fichier, path_fichier exp_id)

REL : 1 expediteur possède n fichiers

# Notes 

** Les fichiers sur ce "template" sont des fichiers suggérés ( base Laravel ) vous pouvez en créer d'autres à votre guise, merci de respecter la syntaxe ** 

__ Proposition d'une étudiante : Envoyer le mail à plusieurs personnes en même temps : Faites attention, ça modifie votre modelisation SQL __

