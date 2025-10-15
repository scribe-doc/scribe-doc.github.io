---
layout: default
title: Découper des fichiers PDF
last_modified_date: 2025-10-14
---
# Découper des fichiers PDF avec le logiciel PDFsam

  &nbsp;   

1. Si PDFsam *(PDF Split and Merge)* n'est pas déjà présent sur l'ordinateur :  
	- Télécharger PDFsam Basic (logiciel libre) : [page de téléchargement de PDFsam Basic](https://pdfsam.org/fr/pdfsam-basic/){:target="_blank"};  
	- Installer PDFsam Basic.   
	  &nbsp;  
    

	Si la découpe doit se faire selon **l'un** de ces modes :  
	• après les pages paires;  
	• après les pages impaires;  
	• après chaque page;  
	• après chaque multiple de *n* (groupes du même nombre de pages, exemple découper le document en groupes de 2 pages)  
	=> Passer directement à **l'étape 5**.  
	{: .cl-fct1}

2. Ouvrir le fichier PDF dans le lecteur PDF de son choix (exemple : Adobe Acrobat, Okular, Firefox.. );  
3. Noter les numéros des pages **après lesquelles découper**, séparés par des **virgules**.
	- Dans Adobe Acrobat par exemple, le numéro de la page affichée est visible en bas à droite :  
	  ![](IMG_PDFsam%20-%20Découper%20des%20fichiers%20PDF_2.png)  
	- Exemple : 
		- pour un document de 538 pages pour lequel on souhaite obtenir un PDF pour chacun des groupes de pages suivants : 1-5  \|  6-123  \|  124-502  \|  503-538
		- il faudra noter ceci : **5,123,502** (découpage après les pages 5, 123 et 502)
4. Fermer le fichier à découper ouvert dans le lecteur PDF.  
     
5. Ouvrir PDFsam  
6. Choisir l'outil "Découper" :  
   ![](IMG_PDFsam%20-%20Découper%20des%20fichiers%20PDF_1.png)  
7. Indiquer le fichier à découper :  
	- Cliquer sur "Sélectionnez PDF";  
	- Naviguer jusqu'au fichier à découper, et cliquer dessus;  
	- Cliquer sur "Ouvrir".  
	  ![](IMG_PDFsam%20-%20Découper%20des%20fichiers%20PDF_3.png)  
   
8. Indiquer les paramètres de découpage :  
	- Si les numéros de page après lesquelles découper ont été notés ci-dessus (étapes 2-3-4) :  
		- Cocher "Après les pages suivantes";  
		- Coller les numéros de pages (séparés par des virgules) dans le champ correspondant.  
		  ![](IMG_PDFsam%20-%20Découper%20des%20fichiers%20PDF_4.png) 
	- Sinon, renseigner l'option adaptée.  
9. Indiquer le dossier dans dans lequel seront créés les nouveaux fichiers PDF :  
	- Dans la section "Paramètres de sortie", cliquer sur "Parcourir..."  
	- Naviguer jusqu'au dossier à découper, et cliquer dessus;  
	- Cliquer sur "Sélectionner un dossier".  
	  ![](IMG_PDFsam%20-%20Découper%20des%20fichiers%20PDF_5.png)  
10. Eventuellement, modifier le préfixe des fichiers qui seront créés : dans la section "Paramètres de noms de fichiers", renseigner le préfixe souhaité.  
    ![](IMG_PDFsam%20-%20Découper%20des%20fichiers%20PDF_6.png)  
  11. Enfin, cliquer sur "Exécuter" pour lancer la fusion. Après quelques instants, "terminé" est affiché.   
     ![](IMG_PDFsam%20-%20Fusionner%20des%20fichiers%20PDF_7%20executer%20fusion.png)  
12. Eventuellement, cliquer sur le bouton "Ouvrir" pour ouvrir le dossier contenant les documents produits, et vérifier le résultat.  
    Remarque : le nombre en début de nom de fichier correspond au numéro de page de début dans le document initial.  
    ![](IMG_PDFsam%20-%20Découper%20des%20fichiers%20PDF_8.png)  

13. Pour procéder à un nouveau découpage de document PDF, cliquer sur le bouton "Vider" en haut, puis reprendre à partir du point 1 ci-dessus.  
    ![](IMG_PDFsam%20-%20Découper%20des%20fichiers%20PDF_7.png)  

---
**Pour aller plus loin :**
- [Documentation officielle de PDFsam Basic](https://pdfsam.org/fr/documentation/#basic-documentation){:target="_blank"}
- Tutoriel [Fusionner des fichiers PDF avec le logiciel PDFsam](PDFsam%20-%20Fusionner%20des%20fichiers%20PDF.html)  