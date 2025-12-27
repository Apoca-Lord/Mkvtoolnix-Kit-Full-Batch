# Mkvtoolnix-Kit-Full-Batch
Pour windows : Ceci est un batch interactif via cmd, qui constitue une interface de gestion et traitement de fichiers vidéo via des outils comme FFmpeg et MKVToolNix (mkvmerge, mkvpropedit, etc.). Telque : l’extraction de sous-titres le remuxing de fichiers vidéo avec nouvelles pistes audios/subs la modification de métadonnées
## Table of Contents 
[Présentation](#présentation) 

[Tutoriel](#tutoriel)
Tutoriel : Mkvtoolnix-Kit-Full
*******************************
🎬 Guide pas-à-pas pour utiliser le batch interactif
1. Préparer les dossiers
Avant de lancer le script, organise tes fichiers :

dossierA → tes vidéos sources (.mkv)

dossierB → pistes audio supplémentaires (même nom que la vidéo)

dossierC → sous-titres (.srt, .ass, .sup)
Exemple : Monde_S01E01_track2.ass

dossierD → polices (fonts), max 78

output → sortie temporaire

output_final → sortie finale (fichiers terminés)

👉 Conseil : renomme tes fichiers avec des noms courts (évite les titres trop longs).


2. Lancer le script
Double-clique sur le fichier batch (.bat).
Un menu interactif apparaît avec des options (1 à 7, ou 9 pour quitter).
Choisis l’action que tu veux faire (exemple : 1 pour extraire des sous-titres).


3. Les principales options
1. Extraction de sous-titres → récupère les sous-titres d’une vidéo.
2. Remux sous-titres + polices → ajoute/remplace des sous-titres et polices.
3. Remux/Demux audio → ajoute ou remplace des pistes audio.
4. Remux audio + subs → garde jusqu’à 2 pistes audio et 2 sous-titres.
5. Modifier nom/langue des pistes → change les métadonnées (titre, langue).
6. Nettoyage des titres internes → supprime le titre interne du MKV.
7. Nettoyage audio/subs → supprime toutes les pistes audio et sous-titres.
9. Quitter → ferme le script.

4. Exemple concret : ajouter un sous-titre
Mets ta vidéo dans dossierA : Monde_S01E01.mkv
Mets ton sous-titre dans dossierC : Monde_S01E01_track2.ass
Lance le script → choisis option 2 (Remux subs/fonts).
Le fichier final apparaît dans output_final.

5. Vérifier le résultat
Après traitement :
Ouvre le fichier avec MKVToolNix GUI.
Vérifie que :
Les pistes audio et sous-titres sont bien présentes.
Les noms/langues des pistes sont corrects.
La synchronisation est bonne (sinon corrige avec --sync).

6. Conseils pratiques
Si un fichier ne sort pas correctement :
Vérifie le nom du fichier (trop long ?).
Vérifie qu’il est bien placé dans le bon dossier.
Traite les fichiers par petits lots (2 à 12 max).
Déplace les fichiers déjà traités dans un sous-dossier pour éviter de les retraiter.



[Téléchargement](#téléchargement)
