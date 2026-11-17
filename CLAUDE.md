# CLAUDE.md — Photo labo (distribution)

Dépôt de distribution du logiciel Photo labo. Le code source est dans le dépôt `Photo_labo_source`
(voir son `CLAUDE.md`).

- Le programme compilé **est versionné ici** : `build.bat` (dépôt source) recopie `dist\Photo Labo`
  dans ce dossier par `robocopy /MIR` (fichiers périmés supprimés ; `.git`, `README.md`, `CLAUDE.md`,
  `.gitignore`, `.gitattributes` préservés). Publier = `git add -A`, commit `vX.Y` (même numéro que
  `APP_VERSION`), push. Les utilisateurs mettent à jour par `git pull`.
- Plus de zip ni de Release GitHub (l'ancienne Release v1.2 éventuelle peut être supprimée).
- `_internal/cv2/cv2.pyd` ≈ 86 Mo : sous la limite GitHub de 100 Mo par fichier (avertissement > 50 Mo).
- L'historique Git grossit à chaque version (binaires) ; nettoyage possible mais il réécrit le dépôt :
  à décider avec l'utilisateur.
