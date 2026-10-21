# Objectifs de sécurité et planification (clauses 6.2 et 6.3)

Document : SMSI-03 · Version 1.0 · Propriétaire : RSSI · Revue : à chaque revue de direction

## 6.2 Objectifs de sécurité de l'information

Les objectifs découlent de la PSSI et des risques identifiés dans l'analyse EBIOS RM. Chacun est mesurable, a un responsable, une échéance et des mesures qui y contribuent.

| Id | Objectif | Indicateur | Cible | Échéance | Responsable | Mesures | Risques |
|---|---|---|---|---|---|---|---|
| O1 | Plus aucun risque à un niveau élevé | Nombre de risques résiduels élevés | 0 | 31/12/2027 | RSSI | Toutes les P1 | CA_01 à CA_07 |
| O2 | Protéger les comptes à privilèges | Part des comptes à privilèges protégés par MFA | 100 % | 31/01/2027 | DSI | M_12 | CA_03, CA_04 |
| O3 | Réduire la réussite du phishing interne | Taux de clic aux simulations de phishing | moins de 5 % | 30/06/2027 | RSSI | M_15 | CA_03 |
| O4 | Pouvoir restaurer le core banking après une attaque | Restauration testée réussie, en moins de 4 heures | 4 tests réussis par an | 31/03/2027 | DSI | M_13 | CA_03, CA_04 |
| O5 | Respecter les délais de notification DORA | Incidents majeurs notifiés dans les délais | 100 % | 31/01/2027 | RSSI | M_16 | CA_01 à CA_04 |
| O6 | Encadrer les prestataires critiques | Contrats critiques conformes à l'article 30 de DORA | 100 % | 31/03/2027 | Achats | M_08, M_09 | CA_02, CA_04, CA_05 |
| O7 | Maîtriser les accès aux données clients | Revues trimestrielles des habilitations réalisées | 4 par an | 31/01/2027 | RSSI | M_06, M_22 | CA_05 |
| O8 | Détecter le blanchiment via les comptes clients | Délai moyen entre alerte et déclaration Tracfin | moins de 30 jours | 31/03/2027 | Conformité | M_19 | CA_06, CA_07 |

Le suivi de ces objectifs se fait avec le [tableau de bord des indicateurs](05-indicateurs.md) et est présenté à chaque [revue de direction](07-revue-de-direction.md).

## 6.3 Planification des changements

Tout changement important du SMSI suit ces étapes :

1. Le demandeur décrit le changement : nouveau prestataire TIC, nouveau produit bancaire, évolution réglementaire, changement d'organisation.
2. Le RSSI évalue l'effet sur les risques et décide si une mise à jour de l'analyse EBIOS RM est nécessaire.
3. Les documents concernés (SoA, PSSI, plan de traitement) sont mis à jour.
4. Le propriétaire du risque approuve le changement.
5. Le changement est présenté à la revue de direction suivante.

Déclencheurs d'une nouvelle analyse de risques : un incident majeur, l'arrivée d'un prestataire TIC critique, une évolution importante du SI, un nouveau produit, une nouvelle exigence réglementaire.
