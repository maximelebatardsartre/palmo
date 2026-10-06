# Palmo Companion

Palmo Companion (Palmo pour les intimes) est un compagnon de bureau gratuit pour les joueurs Steam sous Windows.

Chaque joueur a son **Dekko**, un petit slime cubique qui vit sur ton écran. Il se balade sur la barre des tâches, s'installe sur tes fenêtres, dort la nuit et évolue avec tes vrais exploits Steam : succès, raretés, jeux terminés, genres joués. Il en tire une classe, des traits, des titres et une garde-robe de plus de 170 objets.

## Ce que fait Palmo

- **Dekko sur ton bureau** : glisse-le, taquine-le d'un clic. Un clic droit ouvre sa roue (panneau, lanceur, tes raccourcis, taille, masquer).
- **Zéro impact en jeu** : dès qu'un jeu ou une application plein écran démarre, Dekko disparaît vraiment. Plus de rendu, plus de réseau.
- **Débrief de fin de session** : tes succès de la partie, les plus rares fêtés un par un, l'XP gagnée, la montée de niveau.
- **Genèse** : au premier lancement, Dekko relit toute ta vie de joueur et la rejoue en accéléré.
- **Statistiques** : activité jour par jour depuis la création de ton compte, genres, habitudes, raretés, records.
- **Bibliothèque** : jeux presque finis avec les succès qui manquent, backlog et roulette, jeux abandonnés relancés par une mise à jour.
- **Lanceur rapide** : `Alt + Maj + Espace`, quelques lettres, Entrée, le jeu démarre.
- **Cartes à partager** : ton profil, ta série de connexions, tes récaps du mois et de l'année, tes 100 %, en PNG.
- **Personnalisation** : garde-robe, coloris, auras, émotes, bannières et fonds de carte, gagnés en jouant ou trouvés dans des packs ouverts avec des Palmes, la monnaie du jeu (rien ne s'achète avec de l'argent réel).
- **Défis et passe de saison** : trois défis du jour et trois de la semaine tirés de ta vraie vie de joueur, une boutique du jour, et un passe de saison gratuit de 40 paliers avec un coloris exclusif chaque trimestre.
- **Série de connexions** : chaque jour avec Palmo prolonge ta flamme et rapporte des Palmes.
- **Son et musique** : une musique d'ambiance composée en direct et des petits sons, tout se coupe en un clic.
- **Deuxième écran** : pendant un jeu, Dekko peut veiller sur ton autre écran avec les performances du PC.

## Installation

1. Télécharge le fichier `Palmo.Companion_x.y.z_x64-setup.exe` dans la dernière [release](../../releases/latest).
2. Lance-le. L'installation se fait pour ton seul compte Windows, **sans droits administrateur**.
3. Au premier lancement, Maître Gélatin, le doyen des Dekkos, te guide pas à pas. Compte deux minutes.
4. Palmo se met ensuite à jour tout seul, jamais pendant que tu joues.

### Ta clé Steam

Palmo lit tes jeux et tes succès avec ta propre clé Web API Steam, que tu crées gratuitement sur [steamcommunity.com/dev/apikey](https://steamcommunity.com/dev/apikey). Steam demande un compte non limité et l'authentificateur mobile Steam Guard. Palmo t'accompagne pour la créer.

La clé est rangée dans le gestionnaire d'identification de Windows. Elle n'est écrite dans aucun fichier, et Palmo ne l'envoie qu'à Steam. Tu peux la révoquer à tout moment sur la même page Steam.

Pour voir tes succès, le paramètre « Détails des jeux » de ton profil Steam doit être public. Sans lui, Palmo reste utile : bibliothèque, temps de jeu, backlog et lanceur. Tu peux aussi essayer Palmo avec un profil de démonstration, sans clé.

### Avertissement Windows SmartScreen

L'installeur n'est pas encore signé par un certificat de code : c'est un projet gratuit, et ces certificats sont payants. Windows peut donc afficher « Windows a protégé votre ordinateur ». Pour continuer, clique sur **Informations complémentaires**, puis sur **Exécuter quand même**.

### Antivirus

Palmo lit la liste des programmes en cours et le registre de Steam pour savoir quand tu joues, afin de se cacher. Un antivirus peut trouver ce comportement suspect et signaler un faux positif. Pour vérifier que ton fichier est bien celui publié :

1. Télécharge `SHA256SUMS.txt` dans la même release.
2. Dans PowerShell, lance la commande `Get-FileHash .\Palmo.Companion_x.y.z_x64-setup.exe`.
3. Compare l'empreinte affichée avec celle du fichier : elles doivent être identiques.

Les installeurs sont compilés uniquement par GitHub Actions, jamais sur un ordinateur personnel.

## Confidentialité

Tout reste sur ton ordinateur : aucun serveur, aucun compte, aucune télémétrie. Tu peux exporter ou supprimer toutes tes données en un clic depuis les réglages. Les détails sont dans la [page de confidentialité](CONFIDENTIALITE.md).

## Licence

Palmo est gratuit. Son utilisation est régie par la [licence d'utilisation](LICENCE-UTILISATION.md).

Palmo n'est pas affilié à Valve ni à Steam. Steam est une marque de Valve Corporation.
