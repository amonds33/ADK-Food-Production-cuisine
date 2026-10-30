# ADK Food — Cuisine V4 : suivi horaire et observations audio

Application web installable Android (PWA). Les tâches horaires sont reprises du classeur de production, et sont personnalisables depuis Programmation. Les jours et quantités de production sont également modifiables. Chaque tâche cochée est horodatée localement. Les quantités saisies cochent automatiquement OK quand l’objectif est atteint.

## PDF et audio

Le rapport PDF reprend les quantités, tâches horaires accomplies ou non, et observations écrites. Le fichier audio est enregistré séparément dans IndexedDB de l'appareil : le PDF indique sa présence, mais **n’intègre pas l’enregistrement sonore**. Utiliser le bouton Partager/télécharger l’audio pour l'envoyer séparément. Sur Android, autoriser le microphone. Fonctionne sur HTTPS, pas depuis un simple fichier local pour le micro.

## Déploiement

Décompresser le ZIP, remplacer tous les fichiers du dépôt GitHub Pages `adk-food-cuisine`, confirmer le commit, attendre le déploiement Pages puis rouvrir le site dans Chrome. La version V4 doit apparaître. Faire une sauvegarde JSON avant toute modification majeure. Pas de synchronisation entre appareils. Une désinstallation ou suppression des données du navigateur peut détruire les rapports et enregistrements audio. L’envoi e-mail nécessite une connexion et confirmation via Gmail.

## Point d’attention

Le classeur comporte des quantités contradictoires entre synthèse et jours (Mafé et Graine). Les horaires sont indicatifs et reflètent les fiches journalières, sans arbitrer ces contradictions. Les procédures de refroidissement/températures doivent rester conformes au PMS, ce logiciel ne constitue pas une validation HACCP.
