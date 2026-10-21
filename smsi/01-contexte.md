# Contexte de l'organisation (clause 4)

Document : SMSI-01 · Version 1.0 · Propriétaire : RSSI · Revue : annuelle

## 4.1 Enjeux internes et externes

Orséa Banque est une banque en ligne de 150 collaborateurs qui gère environ 200 000 clients particuliers. Elle n'a aucune agence physique et son système d'information est entièrement hébergé dans le cloud.

**Enjeux externes**

| Enjeu | Effet sur la sécurité de l'information |
|---|---|
| Règlement DORA, applicable depuis le 17 janvier 2025 | Cadre de gestion du risque TIC, notification des incidents majeurs, encadrement des prestataires TIC, tests de résilience |
| Supervision de l'ACPR | Contrôles sur place, sanctions en cas de manquement |
| RGPD | Protection des données personnelles des clients, notification des violations à la CNIL sous 72 heures |
| DSP2 | Authentification forte obligatoire pour les paiements |
| Dispositif LCB-FT | Détection des opérations suspectes, déclarations à Tracfin, conservation des pièces 5 ans |
| PCI DSS, exigé par les réseaux de cartes | Protection des données de carte |
| Menace en hausse sur le secteur financier | Phishing des clients, rançongiciels, recrutement de mules, fraude interne |
| Concurrence entre néobanques | La confiance des clients est un argument commercial ; un incident public a un fort impact sur l'image |

**Enjeux internes**

| Enjeu | Effet sur la sécurité de l'information |
|---|---|
| SI 100 % cloud (AWS, région Paris) | Responsabilité partagée avec l'hébergeur, dépendance forte |
| Core banking loué à un éditeur en SaaS | Risque de chaîne d'approvisionnement, dépendance contractuelle |
| Support client en partie externalisé | Accès humains nombreux aux données clients, rotation du personnel |
| Croissance rapide et culture de start-up | Processus peu formalisés, priorité donnée à la mise sur le marché |
| Maturité de sécurité faible au démarrage | Une seule mesure de sécurité réellement en place (authentification forte des clients) |
| Budget de sécurité à construire | Arbitrages nécessaires en comité exécutif |

## 4.2 Parties intéressées

| Partie intéressée | Attentes | Exigence retenue dans le SMSI | Traitement |
|---|---|---|---|
| ACPR | Conformité à DORA et à la réglementation bancaire | Oui | PSSI, plan de traitement, procédure de notification (M_16) |
| Clients | Fonds et données protégés, service disponible | Oui | Objectifs O1, O4 ; mesures M_01 à M_05 |
| CNIL | Respect du RGPD | Oui | Notification des violations, contrôle 5.34 de l'Annexe A |
| Tracfin | Déclarations de soupçon fiables et rapides | Oui | Surveillance LCB-FT (M_19) |
| Actionnaires et COMEX | Maîtrise du risque, budget tenu, image préservée | Oui | Revue de direction, indicateurs |
| Collaborateurs | Règles claires, outils utilisables | Oui | Charte, sensibilisation (M_15) |
| Hébergeur cloud (AWS) | Clauses contractuelles respectées | Oui | Contrat, contrôle 5.23 |
| Éditeur du core banking | Collaboration sur les mises à jour et les incidents | Oui | Clauses DORA (M_09), tests en préproduction (M_10) |
| Processeur de paiement carte | Respect de PCI DSS et des procédures d'incident | Oui | Clauses DORA (M_09) |
| Prestataire KYC | Données d'identité protégées, détection des faux documents | Oui | KYC renforcé (M_17) |
| Prestataire de support client | Règles d'accès claires | Oui | Moindre privilège (M_06), clauses de sécurité (M_08) |
| Assureur cyber | Niveau de sécurité minimal pour couvrir le risque | Oui | Cyber-assurance (M_21) |
| Réseaux de cartes | Conformité PCI DSS | Oui | Via le processeur de paiement |

## 4.3 Domaine d'application

**Intitulé** : « Le SMSI couvre la plateforme bancaire en ligne d'Orséa Banque : ouverture de compte, tenue des comptes, paiements par carte et virements, relation client et support, ainsi que les systèmes et prestataires qui les supportent. »

**Inclus**

- Processus : entrée en relation (KYC), tenue des comptes, paiements par carte, relation client, pilotage réglementaire
- Systèmes : application mobile et espace web, core banking (SaaS), infrastructure AWS, annuaire et gestion des identités, back-office des conseillers, postes de travail
- Personnes : collaborateurs d'Orséa et prestataires ayant accès au SI
- Sites : bureaux d'Orséa ; centres de données AWS couverts via le contrat (contrôle 5.23)

**Exclus**

| Exclusion | Justification |
|---|---|
| Fonctions RH et comptabilité | Hors des activités bancaires critiques ; leurs accès au SI restent soumis à la PSSI |

**Interfaces et dépendances**

| Interface | Nature | Maîtrise |
|---|---|---|
| AWS | Hébergement de toute l'infrastructure | Contrat, responsabilité partagée |
| Éditeur du core banking | Logiciel en SaaS, mises à jour | Clauses DORA, tests en préproduction |
| Processeur de paiement | Autorisation des paiements par carte | Clauses DORA, certification PCI DSS |
| Prestataire KYC | Vérification d'identité à l'ouverture de compte | Contrat, KYC renforcé |
| Prestataire de support | Agents ayant accès aux comptes clients | Moindre privilège, journalisation, clauses |
| RH et comptabilité (hors périmètre) | Utilisation du SI | Comptes et accès gérés selon la PSSI |

## 4.4 Système de management

Le SMSI suit le cycle « planifier, faire, vérifier, améliorer » :

| Étape | Clauses | Documents |
|---|---|---|
| Planifier | 4, 5, 6 | Ce document, [leadership](02-leadership.md), [objectifs](03-objectifs.md), analyse de risques, [SoA](../livrables/SoA_ISO27001_Orsea_Banque.xlsx) |
| Faire | 7, 8 | [Support](04-support.md), [plan de traitement](../livrables/Plan_de_traitement_Orsea_Banque.xlsx), [PSSI](../livrables/PSSI_Orsea_Banque.pdf) |
| Vérifier | 9 | [Indicateurs](05-indicateurs.md), [audit interne](06-audit-interne.md), [revue de direction](07-revue-de-direction.md) |
| Améliorer | 10 | [Non-conformités et actions correctives](08-amelioration.md) |
