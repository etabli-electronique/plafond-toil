# Plafond étoilé – simulateur

Simulateur pour concevoir un plafond étoilé en lambris PVC : constellations réelles visibles depuis La Réunion, ampoules LED (COB), fibre optique, bandes phosphorescentes, tasseaux et pannes C.

L'outil tient dans un seul fichier, `index.html` (HTML, CSS et JavaScript). Il n'a besoin d'aucun serveur, d'aucune installation ni d'aucune bibliothèque. Seule la police Sora est chargée depuis Google Fonts ; hors connexion, le navigateur la remplace par une police système.

## Fonctions

- Constellations placées d'après leurs coordonnées réelles (ascension droite, déclinaison, magnitude), déplaçables, pivotables et redimensionnables à la souris ou au doigt.
- Composition recommandée : Croix du Sud, Pointeurs, Triangle Austral, Scorpion et Sagittaire à leurs vraies positions, traversés par la Voie lactée en fibre optique.
- Ampoules LED (puissance, flux, angle, température en Kelvin) et fibre optique (nombre de brins, diamètre, puissance et flux du projecteur, Kelvin ou couleur).
- Ciel de fibres : uniforme, Voie lactée, galaxie spirale, nébuleuse, nuages d'étoiles, tourbillon, avec numéro de tirage de 0 à 100 et dispositions mémorisées.
- Structure : lambris, tasseaux, pannes C (réparties ou saisies une par une depuis un mur), table sous le plafond.
- Canaux du module de commande, règles d'affectation et ambiances (Tout allumé, Repas, Soirée…), calques par type de lumière et code couleur de repérage.
- Estimation de l'éclairement de la table (référence « Tout allumé » = 100 %), puissance par ambiance et par canal.
- Plan de pose, plan de perçage (CSV, PNG), fiches de perçage lame par lame imprimables, liste de matériel, estimation des longueurs de câble et de fibre.

## Utilisation en local

Téléchargez `index.html` et ouvrez-le par un double-clic : il fonctionne dans Chrome, Edge, Firefox et Safari, sous Windows, macOS et Linux.

Sur iPad et iPhone, l'app Fichiers affiche le fichier sans exécuter le JavaScript : utilisez la version en ligne (voir ci-dessous).

## Mise en ligne avec GitHub Pages

1. Créez un nouveau dépôt public sur GitHub, par exemple `plafond-etoile`.
2. Déposez-y le contenu de ce dossier (`index.html`, `README.md`, `.nojekyll`) : bouton **Add file → Upload files**, puis **Commit changes**. Le fichier `.nojekyll` commence par un point : s'il n'apparaît pas dans votre explorateur, affichez les fichiers cachés. Il n'est pas indispensable, mais il évite un traitement inutile par GitHub Pages.
3. Dans le dépôt, ouvrez **Settings → Pages**.
4. Sous **Build and deployment**, choisissez **Deploy from a branch**, la branche **main** et le dossier **/ (root)**, puis **Save**.
5. Après une ou deux minutes, le site est disponible à l'adresse `https://<votre-nom-github>.github.io/plafond-etoile/`.

Sur iPad, ouvrez cette adresse dans Safari, puis **Partager → Sur l'écran d'accueil** pour l'utiliser comme une application.

## Sauvegarder et partager une configuration

- Vos réglages sont gardés automatiquement dans le navigateur de chaque appareil.
- Onglet **Sauvegarde** : **Télécharger (.json)** pour sauvegarder la configuration, **Importer un fichier** pour la recharger.
- **Télécharger le simulateur avec ces réglages (.html)** crée un nouveau `index.html` qui s'ouvre directement sur votre configuration. Pour mettre à jour le site, remplacez `index.html` dans le dépôt par ce fichier : toute personne qui ouvre le lien démarre alors sur cette version.

## Limites

Les éclairements, puissances et longueurs de câble ou de fibre sont des estimations à partir des valeurs saisies. Reportez les valeurs exactes de vos fiches techniques et faites valider l'installation électrique par un professionnel.
