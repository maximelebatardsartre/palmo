# Confidentialité

Palmo est conçu pour ne rien envoyer à personne.

## Ce que Palmo ne fait pas

- Pas de serveur Palmo, pas de compte à créer.
- Aucune télémétrie, aucune statistique d'usage, aucun traceur.
- Aucune publicité.

## Ce que Palmo lit sur ton ordinateur

- La valeur de registre de Steam qui indique le jeu en cours, et l'état « plein écran » de Windows, pour se cacher pendant que tu joues.
- La liste des programmes en cours, **seulement** si tu as indiqué des programmes qui doivent masquer Dekko.
- Les fichiers locaux de Steam : comptes connus sur ce PC (pour te proposer le tien), dossiers de bibliothèques, jeux installés, date de dernier lancement.
- Les fenêtres ouvertes (position et taille, jamais leur contenu), pour que Dekko puisse marcher sur leur bord supérieur.

## Ce que Palmo demande à Steam

Avec **ta propre clé Web API Steam**, Palmo interroge directement les serveurs de Steam :

- ton profil public (pseudo, avatar, ancienneté, niveau Steam, badges) ;
- ta bibliothèque et ton temps de jeu ;
- tes succès, leurs noms et leur rareté mondiale ;
- les fiches boutique des jeux (genres, prix actuel, image) ;
- les actualités des jeux que tu n'as pas lancés depuis longtemps.
- seulement si tu ouvres le classement « Amis Steam » de l'onglet Potes : ta liste d'amis Steam et, pour ceux dont le profil est public, leur pseudo, leur avatar, leur niveau Steam et leurs jeux des deux dernières semaines. Rien n'est lu pendant que tu joues, au plus une fois par jour, et ces informations restent sur ton PC.

Au sujet de la clé :

- Elle est rangée dans le **gestionnaire d'identification de Windows**. Elle n'apparaît dans aucun fichier, aucun journal, et n'est envoyée qu'à Steam.
- Elle donne accès en lecture aux informations que Steam expose par cette API. Elle ne permet ni d'acheter, ni de modifier ton compte.
- Tu peux la **révoquer à tout moment** sur la page officielle des clés Steam, ou l'oublier depuis les réglages de Palmo.
- Aucun appel réseau n'a lieu pendant que tu joues.

## Où sont tes données

| Quoi | Où |
| --- | --- |
| Bases de données (une par compte) | `%LOCALAPPDATA%\com.az2up.palmo\profiles` |
| Réglages | `%APPDATA%\com.az2up.palmo\settings.json` |
| Clé Steam | Gestionnaire d'identification de Windows |

Les réglages permettent de tout **exporter** (un fichier JSON lisible) ou de tout **supprimer** en un clic, clé comprise. La désinstallation propose aussi d'effacer les données.

## Cartes à partager

Les cartes sont dessinées sur ton ordinateur. Elles ne quittent ton PC que si tu les copies ou les enregistres pour les partager toi-même.

## Mises à jour

Palmo vérifie au lancement, puis toutes les 6 heures, s'il existe une nouvelle version sur cette page GitHub. Cette vérification ne transmet aucune donnée personnelle. Les mises à jour sont signées et vérifiées avant installation, et ne s'installent jamais pendant que tu joues.
