---
layout: default
title: Télécharger des vidéos en ligne avec Vividl
last_modified_date: 2025-03-17
---

# Télécharger des vidéos en ligne avec Vividl
&nbsp;  
Le logiciel libre Vividl permet de télécharger des vidéos présentes sur des sites comme Youtube ou Dailymotion.

## Installation

1. Accéder au [site officiel de Vividl](https://sourceforge.net/projects/vividl/files/){:target="_blank"}  
2. Télécharger la dernière version. Si vous n'êtes pas administrateur de votre poste, prendre la version portable (exemple : Vividl-v.0.8.0-Portable.zip)  
  ![](IMG_Télécharger%20des%20vidéos%20en%20ligne%20avec%20Vividl_0.png)
3. Décompresser le fichier zip téléchargé
4. Ranger le dossier décompressé (exemple : Vividl-v.0.8.0-Portable) à l'emplacement souhaité (il ne devra ensuite plus être déplacé)  
5. Ouvrir le dossier, faire un clic-droit sur le fichier "Vividl.exe", puis cliquer sur "Epingler au menu Démarrer"
  ![](IMG_Télécharger%20des%20vidéos%20en%20ligne%20avec%20Vividl_1.png)


## Configuration


1. Lancer le logiciel en utilisant l'icone correspondante qui a été ajoutée au menu démarrer  
   ![](IMG_Télécharger%20des%20vidéos%20en%20ligne%20avec%20Vividl_2.png)  
2. Cliquer sur l'icone en forme d'engrenage en haut à droite, afin d'accéder aux paramètres  
   ![](IMG_Télécharger%20des%20vidéos%20en%20ligne%20avec%20Vividl_3.png)  
3. Dans l'onglet "Généralités", pour "Format de téléchargement par défaut", sélectionner "Meilleur téléchargement direct"  
   ![](IMG_Télécharger%20des%20vidéos%20en%20ligne%20avec%20Vividl_5.png)  
4. Si vous utilisez un proxy pour accéder à Internet : dans l'onglet "Télécharger", indiquer l'adresse du proxy  
   ![](IMG_Télécharger%20des%20vidéos%20en%20ligne%20avec%20Vividl_6.png)  
5. Enfin, cliquer sur "D'accord" en bas de la fenêtre pour valider.   
   ![](IMG_Télécharger%20des%20vidéos%20en%20ligne%20avec%20Vividl_7.png)
  
Le logiciel est à présent prêt à être utilisé.

## Utilisation

1. Copier l'adresse de la page contenant la vidéo  
   *&nbsp; Exemple avec l'adresse du clip du prix Non au Harcèlement 2023-2024 :  
   &nbsp; https://www.youtube.com/watch?v=jb32LNQ9eBo*
2. Dans Vividl, cliquer sur l'icone en forme d'éclair;
3. Après quelques instant, les informations de la vidéo ont été récupérées. Cliquer sur le bouton de téléchargement à droite pour lancer le téléchargement de la vidéo  
   ![](IMG_Télécharger%20des%20vidéos%20en%20ligne%20avec%20Vividl_8.png)  
4. Une fois la vidéo téléchargée, cliquer sur l'icone en forme de dossier à droite pour ouvrir le dossier contenant la vidéo.  
   ![](IMG_Télécharger%20des%20vidéos%20en%20ligne%20avec%20Vividl_9.png)  

## \[MAJ 17/03/2025\] Mise à jour manuelle de yt-dlp

Vividl utilise le programme yt-dlp pour télécharger les vidéos en ligne.  
Cependant, au 17/03/2025, la version de yt-dlp embarquée par la dernière version disponible de Vividl (0.8.0) n'est plus à jour. Vividl intègre un mécanisme de mise à jour de yt-dlp, mais celui-ci ne semble pas fonctionner si un proxy est requis pour accéder à internet.  
Cette version "périmée" de yt-dlp entraine l'échec du téléchargement des vidéos.  

Pour résoudre ce problème, il est nécessaire de mettre à jour yt-dlp manuellement.  
Pour cela :   
- Télécharger la dernière version de yt-dlp.exe présente sur la [page de téléchargement de yt-dlp](https://github.com/yt-dlp/yt-dlp/releases){:target="_blank"};   
  ![](IMG_Télécharger%20des%20vidéos%20en%20ligne%20avec%20Vividl_10.png)
- Se rendre dans le dossier du logiciel Vividl (par exemple : "Vividl-v.0.8.0-Portable"), dans le sous-dossier "Lib", puis écraser le fichier "yt-dlp.exe" présent par celui téléchargé ci-dessus.  
  Par exemple, si les fichiers du programme Vividl se trouvent dans le dossier   
  "C:\Users\utilisateur\Programmes\Vividl-v.0.8.0-Portable\\",  
  copier le fichier yt-dlp.exe téléchargé dans le dossier  
  "C:\Users\utilisateur\Programmes\Vividl-v.0.8.0-Portable\Lib\\"  :  
  ![](IMG_Télécharger%20des%20vidéos%20en%20ligne%20avec%20Vividl_11.png)
   