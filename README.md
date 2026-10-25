# Journal alimentaire

Une petite appli pour photographier chacun de ses repas, puis envoyer une synthèse du jour ou de la semaine à sa diététicienne.

**Rien ne quitte le téléphone.** Les photos sont enregistrées uniquement dans le téléphone. Il n'y a ni compte, ni serveur, ni publicité, ni statistiques de visite. Les photos ne partent que lorsque vous envoyez vous-même une synthèse (WhatsApp, mail, SMS…).

## Installer l'appli

**Android (Chrome)**
1. Ouvrez l'adresse de l'appli dans Chrome.
2. Touchez « Installer l'appli » dans l'onglet Sauvegarde, ou passez par le menu ⋮ puis « Ajouter à l'écran d'accueil ».

**iPhone (Safari)**
1. Ouvrez l'adresse de l'appli dans Safari.
2. Touchez le bouton Partager (le carré avec une flèche), puis « Sur l'écran d'accueil », puis Ajouter.
3. Ensuite, ouvrez toujours le journal depuis son icône. Les photos prises dans Safari ne se retrouvent pas dans l'appli installée.

## Au quotidien

- **Journal** : une photo à chaque repas, avec un commentaire si vous le souhaitez.
- **Synthèse** : une image du jour ou de la semaine, à envoyer à votre diététicienne. Dans WhatsApp, touchez « HD » avant d'envoyer pour que l'image reste nette. Vous pouvez aussi l'enregistrer, puis l'envoyer comme Document.
- **Sauvegarde** : exportez de temps en temps vos photos dans un fichier. Si vous changez de téléphone ou si le navigateur est vidé, c'est le seul moyen de les récupérer. C'est aussi dans cet onglet que vous pouvez supprimer les anciennes photos déjà envoyées.

## Technique

Il s'agit d'une page web installable (PWA) tenant dans un seul fichier `index.html`, sans dépendance. Les photos sont stockées dans IndexedDB, et un service worker (`sw.js`) permet d'ouvrir l'appli hors connexion. Pour publier une mise à jour, il faut changer `VERSION` dans `sw.js`.

Licence MIT : voir `LICENSE`.
