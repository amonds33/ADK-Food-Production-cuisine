# ADK Food — Production cuisine (PWA V1)

Application indépendante de la check-list des stocks avant service.

## Utilisation
- Onglets **Lundi à Dimanche**, regroupés par semaine (sélectionnez une date pour changer de semaine).
- Objectifs de production personnalisables pour chaque jour (onglet « Objectifs »).
- Quantité « Réalisé » saisie pour chaque préparation ; case **OK cochée automatiquement** quand réalisé >= objectif strictement positif.
- Quantités enregistrées immédiatement sur l'appareil dans le stockage du navigateur ; responsable/notes enregistrés à la modification ou par « Enregistrer le jour ».
- Export CSV, sauvegarde JSON, restauration JSON.
- Bouton « Envoyer le rapport » : ouvre l'application e-mail avec le rapport prérempli à **contact@adk-food.fr**. L'utilisateur confirme l'envoi ; une connexion Internet est nécessaire.

## Objectifs initiaux
Certains produits ont des valeurs initiales **indicatives**, issues d'échanges sur la préparation de plats en semaine. Le vendredi et samedi, +3 sur ces produits ; **tout objectif doit être vérifié dans « Objectifs » avant exploitation**. Les autres objectifs sont non définis et ne déclenchent pas de validation automatique tant qu'ils ne sont pas renseignés.

## Déploiement sur GitHub Pages
1. Créer **un nouveau dépôt** GitHub public, par exemple `adk-food-cuisine` (ne pas écraser le dépôt existant de la check-list avant service).
2. Décompresser le ZIP puis importer **le contenu** du dossier au niveau racine du dépôt (index.html à la racine).
3. Settings → Pages → Deploy from a branch → `main` → `/(root)` → Save.
4. Sur Android, ouvrir l'URL fournie, puis Chrome → ⋮ → Installer l'application / Ajouter à l'écran d'accueil.
5. Après installation et un premier chargement réseau, l'application peut fonctionner hors ligne. Les e-mails nécessitent Internet.

## Limites et sécurité
- Les données restent **uniquement sur l'appareil** : pas de synchronisation téléphone/tablette et risque de perte si données navigateur supprimées. Faire des sauvegardes JSON régulièrement.
- Le code GitHub Pages est public. Les saisies locales ne sont pas publiées par défaut.
- Le bouton e-mail ne prouve pas la livraison : le responsable doit finaliser l'envoi depuis son client e-mail.
- Les quantités des différents jours sont indépendantes : cette application gère **la production réalisée**, pas un inventaire en temps réel ni une traçabilité HACCP complète.
