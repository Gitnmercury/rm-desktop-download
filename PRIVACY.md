# Confidentialité et données

**En résumé : tout reste sur votre PC et votre tablette. Rien n'est envoyé à l'auteur.**

## Ce que le logiciel ne fait pas

- Aucune collecte de données, aucun compte, aucun cloud.
- Aucune télémétrie, aucune statistique d'usage.
- Aucun appel réseau automatique vers Internet. « Vérifier les mises à jour » ouvre seulement la
  page de téléchargement dans votre navigateur, à votre demande.

## Échanges avec la tablette

Le logiciel ne communique qu'avec votre tablette reMarkable, branchée en USB (adresse locale
10.11.99.1), par SSH et, si elle est activée, par l'interface web USB de la tablette.

## Clé SSH

Au premier lancement, une clé de connexion est générée sur votre PC :
`%USERPROFILE%\.ssh\id_rm` (clé privée) et `id_rm.pub` (clé publique, copiée sur la tablette).
La clé privée ne quitte jamais votre PC.

## Mot de passe de la tablette

S'il est mémorisé, il est chiffré :

- sous Windows avec DPAPI : seul votre compte Windows, sur ce PC, peut le déchiffrer ;
- sous Linux (version Python) : scellé avec l'identifiant de la machine, dans un fichier
  accessible à votre seul compte.

Il est stocké dans `%APPDATA%\rM Desktop\settings.json` (application Windows) ou
`~/.rm_manager.json` (version Python). « Aide › Oublier le mot de passe mémorisé » l'efface.

## Sauvegardes

Les sauvegardes `.rmbak` sont chiffrées sur votre PC. Ni le logiciel ni l'auteur ne détiennent de
copie de leurs clés.

## Journaux de diagnostic

« Aide › Exporter les journaux de diagnostic » crée un fichier texte local, que vous seul décidez de
transmettre. Il contient : version et build du logiciel, version de Windows et d'OpenSSH, état de la
connexion, réglages d'affichage, derniers messages d'état et erreurs.

Il **ne contient jamais** : mot de passe (même chiffré), clé SSH, clé de sauvegarde, contenu ou noms
de vos documents.

## Contact

apps@ohtna.fr - Anthony BELKACEM EI
