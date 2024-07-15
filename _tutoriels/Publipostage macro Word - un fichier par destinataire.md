---
layout: default
title: "[Bureautique] Word : Publipostage avec un document par destinataire (macro Word)"
last_modified_date: 2024-07-10
---
# Comment obtenir un document par destinataire lors d'un publipostage sous Word
## Introduction  
&nbsp;  
Le résultat d'un publipostage sous Word est habituellement un unique fichier contenant tous les courriers.  
Cependant, il peut arriver que l'on souhaite obtenir comme résultat un fichier par courrier (par exemple pour le transmettre de manière dématérialisée au destinataire).

La macro proposée ci-dessous peut être ajoutée à Word, afin d'obtenir un fichier DOCX et un fichier PDF pour chaque destinataire d'un publipostage.

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
  
- Double-cliquer sur le nouveau module ("Module1") pour afficher son contenu (vide), et coller dedans le contenu (le code/texte) de la [macro de publipostage](/assets/autres/macro découpe publipostage v4.txt){:target="_blank"}.  
- Enregistrer, puis fermer la fenêtre Visual Basic.  
### Ajouter le raccourci vers la macro  
- A droite de la barre de titre, cliquer sur la petite flèche permettant de personnaliser la barre d'outils Accès rapide, et cliquer sur "Autres commandes";  
  ![](IMG_Publipostage%20macro%20Word%20-%20un%20fichier%20par%20destinataire%204.jpg)  
- Dans la liste déroulante de gauche, sélectionner "Macros", cliquer sur la macro DecoupePublipostage juste en dessous, puis cliquer sur "Ajouter >>";  
  ![](IMG_Publipostage%20macro%20Word%20-%20un%20fichier%20par%20destinataire%205.jpg)
- Cliquer enfin sur OK pour valider.   
  La macro pourra ainsi être lancée par la suite depuis l'icone présente dans la barre d'Accès rapide :  
  ![](IMG_Publipostage%20macro%20Word%20-%20un%20fichier%20par%20destinataire%206.jpg)

## Utilisation

*(à venir)*  

