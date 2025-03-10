---
layout: default
title: "[E-mail] Publipostage par mail avec Thunderbird"
last_modified_date: 2025-03-10
---
# Comment faire un publipostage par mail avec avec Thunderbird et l'extension Mail Merge ?

*Remarque : Le tutoriel ci-dessous explique comment effectuer un publipostage avec Mail Merge, sans pièce jointe spécifique à chaque destinataire.*
## Introduction
*Mail Merge* est un addon (module complémentaire, extension) pour Thunderbird permettant de faire du publipostage mail. Comme avec un publipostage classique sur Word/Writer, on utilise une source de données (fichier XLSX ou CSV créé avec Excel ou Calc, par exemple).  
Cette source de données va contenir les informations spécifiques à chaque mail (une ligne = un mail). Par exemple : adresse e-mail du destinataire, nom, prénom, pièce jointe spécifique …  
Cette source de données est associée un modèle de mail, qui servira de base pour chaque e-mail envoyé.  
## Installation de l'extension Mail Merge pour Thunderbird

[L’addon Mail Merge](https://addons.thunderbird.net/fr/thunderbird/addon/mail-merge/){:target="_blank"} doit être installé avant de continuer. Ce guide est basé sur la version 10.5.0.  
- Dans Thunderbird, cliquer sur l'icone du menu en haut à droite, puis cliquer sur "Modules complémentaires et thèmes";  
  ![](IMG_Thunderbird%20-%20Publipostage%20mail%20avec%20Mail%20Merge_16.png)
- La liste des Extensions installées est affichée.  
  Si l'extension Mail Merge n'y figure pas déjà (car non installée), faire une recherche en ligne pour l'extension "Mail Merge" en utilisant le champ de recherche en haut à droite;  
  ![](IMG_Thunderbird%20-%20Publipostage%20mail%20avec%20Mail%20Merge_17.png)
- Dans la liste des résultats, cliquer sur "Mail Merge" (*et non pas "Mail Merge P"*);  
  ![](IMG_Thunderbird%20-%20Publipostage%20mail%20avec%20Mail%20Merge_18.png)
- Vérifier qu'il s'agit de l'extension "Mail Merge" "Alexander Bergmann", puis cliquer sur "Ajouter à Thunderbird". Confirmer si besoin.  
  ![](IMG_Thunderbird%20-%20Publipostage%20mail%20avec%20Mail%20Merge_1.png){:width="500px"}    
  L'extension Mail Merge est à présent installée.  
En cas de besoin, consulter la page [Installer une extension sur Thunderbird (mozilla.org)](https://support.mozilla.org/fr/kb/installer-une-extension-sur-thunderbird){:target="_blank"}.  

## Utilisation
### Préparer la source de données

Préparer le classeur Excel/Calc (source de données) contenant les informations de chaque destinataires.  
Des exemples de sources de données sont disponible : [Fichiers d'exemple de tableau pour Mail Merge](/assets/autres/Fichiers exemple Mail Merge Thunderbird.zip).
Exemple :  
![](IMG_Thunderbird%20-%20Publipostage%20mail%20avec%20Mail%20Merge_2.png)  


Pour créer ce tableau : 
- Ouvrir la première feuille d'un classeur (plus simple pour commencer);
- Sur la **ligne 1**, renseigner le titre de chaque colonne (information), par exemple « MailDestinataire » (caractères alphanumériques uniquement, **sans espaces**);   
  *Remarque : la seule information obligatoire est l'adresse e-mail du destinataire*
- Sur **les lignes suivantes**, renseigner les informations de chaque destinataire;
- Enfin, enregistrer le classeur au **format XLSX** (le format CSV est possible mais nécessite de préciser des paramètres supplémentaires par la suite).  
  
### Préparer le modèle de mail 
- Dans Thunderbird, créer un nouveau message (ou repartir d’un modèle/courriel existant) ;
- Renseigner l'expéditeur et le sujet;
- Renseigner le corps de mail;
- Concernant les éventuelles pièces jointes (collectives) :
	- Idéalement, déposer les pièces jointes sur un espace de stockage temporaire, et ne mettre que le lien dans l'e-mail;
	- Si les pièces sont très légères, il est possible de les ajouter en pièces jointes. Mais de manière générale c'est à éviter pour ne pas surcharger les boites mail.
- Ajouter le destinataire du mail : 
	- dans le champ "Pour" (destinataire), saisir "\{\{MailDestinataire\}\}" (nom de la colonne des adresse mail, entouré de deux accolades de chaque côté);
	- puis valider avec la touche Tabulation ou la touche Entrée du clavier.
- Ajouter les éventuelles informations complémentaires spécifiques à chaque destinataire, si nécessaire : pour cela, saisir le nom de la colonne correspondante, entourée de 2 accolades (comme pour le destinataire), à l'emplacement souhaité dans le corps du mail et/ou dans l'objet du mail.   

Exemple :  
![](IMG_Thunderbird%20-%20Publipostage%20mail%20avec%20Mail%20Merge_3.png)

### Générer les e-mail individuels
1. Ouvrir Mail Merge en utilisant l'une de ces deux méthodes :  
   *Remarque: dans les deux cas, une copie du mail sera alors enregistrée dans le dossier "Modèles".*
	- Soit en cliquant sur le bouton "Mail Merge" dans la barre d'outils;  
	  ![](IMG_Thunderbird%20-%20Publipostage%20mail%20avec%20Mail%20Merge_4.png)
	- Soit en allant de le menu "Outils" puis  "Mail Merge".![](IMG_Thunderbird%20-%20Publipostage%20mail%20avec%20Mail%20Merge_5.png)
2. Renseigner les informations demandées : 
	- Pour la valeur "Source", sélectionner "XLSX";
	- Pour la valeur "Fichier", cliquer sur "Parcourir...", puis sélectionner la source de données (fichier Excel préparé précédemment);
	- Pour la valeur "Mode de livraison", sélectionner "Envoyer plus tard";  
	  *En sélectionnant ce mode de livraison, les e-mail seront d'abord créés dans un dossier pour être revus, ce qui permet de vérifier leur contenu avant leur envoi.*
	- ![](IMG_Thunderbird%20-%20Publipostage%20mail%20avec%20Mail%20Merge_6.png)
3. Vérifier que la source données est correctement chargée :
	- En bas à droite de la fenêtre, cliquer sur "Fichier";  ![](IMG_Thunderbird%20-%20Publipostage%20mail%20avec%20Mail%20Merge_7.png)
	- Vérifier que les données de la source de données sont correctement affichées. Si besoin, utiliser la barre de défilement en bas pour faire apparaitre les colonnes de droite. Enfin, fermer la fenêtre à l'aide de la croix en haut à droite.  
	  ![](IMG_Thunderbird%20-%20Publipostage%20mail%20avec%20Mail%20Merge_9.png)
4. Vérifier l'édition correcte d'un message :
	- En bas à droite de la fenêtre, cliquer sur "Message";
	  ![](IMG_Thunderbird%20-%20Publipostage%20mail%20avec%20Mail%20Merge_7.png)
	- Vérifier que l'expéditeur est correct, ainsi que le destinataire, le sujet, et les éventuelles autres informations insérées dans l'e-mail. Toutes les valeurs entre doubles accolades doivent avoir été remplacées.  
	  ![](IMG_Thunderbird%20-%20Publipostage%20mail%20avec%20Mail%20Merge_10.png)
	- Une fois cette vérification effectuée, fermer la fenêtre en utilisant la croix en haut à droite.
5. Générer les e-mails individuels
	- Cliquer sur "Envoyer" en bas à droite;  
	  ![](IMG_Thunderbird%20-%20Publipostage%20mail%20avec%20Mail%20Merge_8.png)
	- Dans la fenêtre qui s'affiche, vérifier que la valeur affichée pour "Total" correspond au nombre de destinataires dans la source de données;
	- Puis cliquer sur "Démarrer" pour lancer la création des e-mails individuels;  
	  ![](IMG_Thunderbird%20-%20Publipostage%20mail%20avec%20Mail%20Merge_11.png)
	- Une fois que les courriers ont été créés par Mail Merge, ses fenêtres se ferment.

### Vérifier et envoyer les e-mails individuels générés par Mail Merge
- Dans la fenêtre principale de Thunderbird, cliquer sur le dossier local "Messages en attente" (les dossiers locaux sont habituellement situés en dessous des autres boites mail).  
  ![](IMG_Thunderbird%20-%20Publipostage%20mail%20avec%20Mail%20Merge_12.png)  
  La liste des messages générés est alors affichée.  
  ![](IMG_Thunderbird%20-%20Publipostage%20mail%20avec%20Mail%20Merge_13.png)
- Vérifier que le nombre de message en attente correspond au nombre de messages attendus (nombre de destinataires du tableau).  
  *Remarque : cela n'est valable que s'il n'y avait pas déjà des messages en attente dans ce dossier.*
- Pour le premier message, le dernier, ainsi qu'éventuellement quelques autres, vérifier que leur contenu est correct (expéditeur, destinataire, sujet, corps du message).  
  ![](IMG_Thunderbird%20-%20Publipostage%20mail%20avec%20Mail%20Merge_15.png)
- Enfin, précéder à l'envoi : faire un clic droit sur le dossier "Messages en attente", puis cliquer sur "Envoyer les messages non envoyés".  
  ![](IMG_Thunderbird%20-%20Publipostage%20mail%20avec%20Mail%20Merge_14.png)  
  *Les messages vont alors être envoyés un par un.*  
  *Une copie des messages envoyés sera placée dans le dossier "Messages envoyés" de la boite mail associée à l'adresse d'envoi (ou dans le dossier "Messages envoyés" des dossiers locaux si cette boite n'est pas présente dans Thunderbird).*
