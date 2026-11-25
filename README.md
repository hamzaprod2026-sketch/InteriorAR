# Interior’AR — Site vitrine + CRM (prototype frontend)

Projet de démonstration réalisé en HTML5, CSS3 et JavaScript Vanilla.

## Lancer le projet
1. Décompresser l’archive.
2. Ouvrir `index.html` dans un navigateur. Pour un fonctionnement plus fiable, utiliser l’extension Live Server de VS Code.
3. Aller dans Contact et envoyer une demande de test.
4. Ouvrir `crm/login.html` dans le même navigateur et la même origine.
5. Se connecter avec les identifiants ci-dessous.

## Identifiants CRM de démonstration
- E-mail : `admin@interiorar.demo`
- Mot de passe : `InteriorAR2026`

## Fonctionnement
- Les demandes du formulaire public sont enregistrées dans `localStorage` sous la clé `interiorar_requests`.
- Le CRM lit et modifie les mêmes données.
- Les statuts, notes et suppressions sont simulés dans le navigateur.
- La session de connexion est simulée avec `sessionStorage`.

## Limites importantes
- Il s’agit d’un prototype frontend, PAS d’un CRM sécurisé ni d’un système de production.
- LocalStorage est propre au navigateur et à l’origine : les demandes ne sont pas partagées entre plusieurs appareils ou utilisateurs.
- Aucun envoi d’e-mail, aucun upload réel de fichier, aucun backend, aucune API et aucune base de données.
- Les images utilisées sont des images d’inspiration chargées depuis Unsplash (connexion Internet requise). Elles ne sont pas des photographies de réalisations Interior’AR.
- Les articles affichés sont des exemples éditoriaux, pas des articles officiels vérifiés.
- Les fiches de projets et certaines catégories sont à confirmer. Les titres des projets sont repris de l’inventaire initial, mais les galeries et détails originaux n’ont pas été fournis dans les ressources de départ.
- Les coordonnées du site actuel doivent être vérifiées : des variantes apparaissent selon les pages.
- Compléter les contenus et remplacer les images d’inspiration par les photographies originales avant toute présentation comme site définitif ou publication.

## Structure
- `index.html` : accueil
- `pages/` : à propos, services, portfolio, détail projet, blog, contact
- `crm/` : connexion, tableau de bord, demandes, clients
- `css/` : styles du site et du CRM
- `js/` : données de démonstration, interactions et CRM
- `assets/images/` : dossier réservé aux images locales officielles

## Personnalisation
Les projets et contenus de démonstration se trouvent dans `js/data.js`. Le formulaire et le CRM partagent la même clé LocalStorage définie dans `js/main.js` et `js/crm.js`.


## Mise à jour Portfolio

- Le menu public utilise désormais le libellé « Portfolio ».
- Les 12 entrées du portfolio sont présentes avec une fiche individuelle. La fiche The Roxanne Residence reprend les informations fournies dans la capture : programme, maître d’ouvrage, localisation, durée et période d’exécution.
- Les seules métadonnées techniques affichées sont celles récupérées dans la fiche officielle de « La Canada de Tanger » (programme, propriétaire, adresse, durée, surface et période). Pour les autres entrées, le site officiel consulté ne rendait pas de descriptif textuel détaillé accessible ; aucune donnée n'a été inventée.
- Les photographies de la maquette restent des images d'illustration Unsplash et ne sont pas les visuels officiels des réalisations.
- Le bouton « Espace admin » est ajouté à côté du bouton de devis.
- La déconnexion du CRM renvoie désormais vers la page d'accueil publique.
