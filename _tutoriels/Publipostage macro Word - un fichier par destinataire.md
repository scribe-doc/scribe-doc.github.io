---
layout: default
title: "[Bureautique] Word: Publipostage avec un document par destinataire (macro Word)"
last_modified_date: 2025-03-04
---
# Comment obtenir un document par destinataire lors d'un publipostage sous Word

## Introduction  
&nbsp;  
Le résultat d'un publipostage sous Word est habituellement un unique fichier contenant tous les courriers.  
Cependant, il peut arriver que l'on souhaite obtenir comme résultat un fichier par courrier (par exemple pour le transmettre de manière dématérialisée au destinataire).

La macro proposée ci-dessous peut être ajoutée à Word, afin d'obtenir un fichier DOCX et un fichier PDF pour chaque destinataire d'un publipostage.  
Elle a été testée sur Office 2016, mais devrait vraisemblablement fonctionner aussi sur les versions plus récentes.

## Installation

### Activer l'onglet développeur (dans Word)  
 - Cliquer sur "Fichier" en haut à gauche ;  
 - Cliquer sur "Options" à gauche ;  
 - Dans la rubrique "Personnaliser le ruban", à droite, cocher "Développeur", puis valider.  
   ![](IMG_Publipostage%20macro%20Word%20-%20un%20fichier%20par%20destinataire%201.jpg)  

### Ajouter la macro  
- Dans l'onglet "Développeur", cliquer sur "Visual Basic";  
  ![](IMG_Publipostage%20macro%20Word%20-%20un%20fichier%20par%20destinataire%203.jpg)
- Dans la nouvelle fenêtre, à gauche, clic-droit sur "Normal" > "Insertion" > "Module";  
  ![](IMG_Publipostage%20macro%20Word%20-%20un%20fichier%20par%20destinataire%202.png)
  
- Double-cliquer sur le nouveau module ("Module1") pour afficher son contenu (vide), et coller dedans le contenu (le code/texte) de la [macro de publipostage](/assets/autres/macro découpe publipostage v6.txt){:target="_blank"}.  
- Enregistrer, puis fermer la fenêtre Visual Basic.  
### Ajouter le raccourci vers la macro  
- A droite de la barre de titre, cliquer sur la petite flèche permettant de personnaliser la barre d'outils Accès rapide, et cliquer sur "Autres commandes";  
  ![](IMG_Publipostage%20macro%20Word%20-%20un%20fichier%20par%20destinataire%204.jpg)  
- Dans la liste déroulante de gauche, sélectionner "Macros", cliquer sur la macro "DecoupePublipostage" juste en dessous, puis cliquer sur "Ajouter >>";  
  ![](IMG_Publipostage%20macro%20Word%20-%20un%20fichier%20par%20destinataire%205.jpg)
- Cliquer enfin sur OK pour valider.   
  La macro pourra ainsi être lancée par la suite depuis l'icone présente dans la barre d'Accès rapide :  
  ![](IMG_Publipostage%20macro%20Word%20-%20un%20fichier%20par%20destinataire%206.jpg)

## Utilisation
### Préparer les documents Word et Excel

- **Commencer par créer un publipostage classique** : créer le fichier Excel contenant les destinataires, puis le modèle Word, et enfin utiliser l'Assistant Fusion et publipostage de Word. Prévisualiser les courriers et vérifier qu'ils correspondent à ce qui est attendu.   
Ne pas cliquer sur "Terminer & fusionner" (ou fermer le document produit pour revenir au modèle Word).  
Si besoin, de nombreuses ressources sur internet expliquent comment créer un publipostage avec Word et Excel. Par exemple : 
	- [Utiliser le publipostage pour personnaliser des lettres (microsoft.com)](https://support.microsoft.com/fr-fr/office/utiliser-le-publipostage-pour-personnaliser-des-lettres-d7686bb1-3077-4af3-926b-8c825e9505a3){:target="_blank"}  
	- [Comment faire du publipostage avec Word et Excel (laminuteexcel.com)](https://laminuteexcel.com/comment-faire-du-publipostage-avec-excel-et-word/){:target="_blank"}  
&nbsp;    
- Remarques : 
	- Valeurs identiques : si certaines lignes ont la même valeur dans la colonne A, ces lignes doivent *impérativement* se suivre. Ceci peut être fait en triant le tableau par la colonne A, par exemple.
	- Nommage des fichiers :
		- Les courriers individuels seront nommés ainsi :  
		   \<valeur colonne A\>-\<nom du modèle Word\>.\<extension\>
		- Par exemple, si la colonne A comporte la valeur "Pierre MARTIN" pour le premier destinataire (ligne 2), et que le modèle Word se nomme "Courrier bourse.docx", les fichiers correspondant à ce destinataire seront nommés ainsi :
			- "Pierre MARTIN-Courrier bourse.docx"
			- "Pierre MARTIN-Courrier bourse.pdf"
		- Aussi, il est conseillé de choisir le nom du modèle Word, et le contenu de la colonne A du tableau, en fonction des noms de sortie souhaités.

### Générer les courriers individuels


- Une fois le publipostage prêt, **cliquer sur l'icone de lancement de la macro de publipostage** située dans la barre de titre :  
  ![](IMG_Publipostage%20macro%20Word%20-%20un%20fichier%20par%20destinataire%206.jpg)  
  Les courriers vont alors être générés un par un.  
Dans le dossier dans lequel se trouve le modèle Word, un sous-dossier "Publipostage" est créé automatiquement par la macro. Les courriers individuels sont créés dans ce dossier (deux fichiers par destinataire : un fichier PDF et un fichier DOCX).