# Mkvtoolnix-Kit-Full-Batch
Pour windows : Ceci est un batch interactif via cmd, qui constitue une interface de gestion et traitement de fichiers vidéo via des outils comme FFmpeg et MKVToolNix (mkvmerge, mkvpropedit, etc.). Telque : l’extraction de sous-titres le remuxing de fichiers vidéo avec nouvelles pistes audios/subs la modification de métadonnées

## [Présentation](#présentation) 
Voici une synthèse explicative de ce script batch interactif, qui constitue une interface de gestion et traitement de fichiers vidéo via des outils comme FFmpeg et MKVToolNix (mkvmerge, mkvpropedit, etc.).
<br/>
🎯 But principal du script
Créer un outil interactif en ligne de commande pour automatiser des opérations courantes sur les fichiers .mkv, comme :
- l’extraction de sous-titres
- le remuxing (réassemblage) de fichiers vidéo avec nouvelles pistes audios/subs
	- Ajout de sous-titres et de polices
	- Remplacement ou ajout de pistes audio
- le nettoyage de métadonnées
- la modification des noms/langues des pistes
<br/>

🔧 Fonctionnement global
Extraire le dossier compressé pour l'utiliser n'importe où.

Exécuter le menu interactif avec des options de traitement
Menu : L'utilisateur choisit une tâche (1 à 7, ou 9 pour quitter)
Chaque tâche mène à un sous-menu ou appelle un script .bat/.ps1

<br/>

🗂️ Organisation des dossiers
bin\ : Contient les exécutables nécessaires (ffmpeg.exe, mkvmerge.exe, etc.)
- dossierA : Dossier des fichiers vidéo source
- dossierB : Dossier des pistes audio supplémentaires
- dossierC : Dossier des sous-titres à ajouter/remplacer
- dossierD : Dossier des polices (fonts)
- output\ : Dossier temporaire de sortie (traitement)
- output_final\ : Dossier final de sortie
<img src="https://zupimages.net/up/25/52/wae0.jpg" alt="Visuel principal" style="max-width:100%;width:600px;height:auto;">

<br/>

📌 Explication des options du menu
1. Extraction de sous-titres (.ass, .srt, .sup)
Choix entre extraction via cmd ou PowerShell (pour réseau)

2. Remux de sous-titres et polices
	- Remplacement total (Remux)
	- Ajout simple (pas de remplacement)
	- Opération combinée subs + fonts

3. Remux / Demux audio
	- Remplace les pistes audio existantes par celles du dossierB
	- Permet d’ajouter ou retirer des pistes audio (et optionnellement un sous-titre)

4. Remux sources audio + subs
Garde jusqu’à 2 pistes audio et 2 sous-titres des fichiers sources

5. Changer nom/langue des pistes
Modifie les métadonnées des pistes audio et/ou sous-titres (titre, langue)

6. Nettoyage des titres internes
Supprime ou modifie le titre interne d’un fichier MKV

7. Nettoyage des pistes audio et sous-titres
Supprime toutes les pistes audio et sous-titres des fichiers sources
(Prépare les fichiers pour un nouveau traitement)

9. Quitter - Ferme proprement le script

<br/>

📚 En résumé
Ce script est une interface interactive pour automatiser le traitement de vidéos MKV (en masse), en s’appuyant sur des outils open source.
Étant imparfait, l'inconvénient principal est : <br/>
Limite de tâches , remux à renouveller en fonctione de la limite de charactère de chaque fichier et du nombre de têches exécuter en une seul fois

<br/>

## [Tutoriel](https://github.com/Apoca-Lord/Mkvtoolnix-Kit-Full-Batch/blob/main/Tutoriel)

<br/>

## [Téléchargement](https://github.com/Apoca-Lord/Mkvtoolnix-Kit-Full-Batch/releases/tag/Master-folder)

<br/>

## [Libre d'utilisation](#Info) <br/>
L'essemble de ce projet à été fait avec l'aide d' l'IA : coopilot et Chatgpt
Ce projet entièrement gratuit et libre d'accé.

