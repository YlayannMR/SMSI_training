# Surveillance et mesure (clause 9.1)

Document : SMSI-05 · Version 1.0 · Propriétaire : RSSI · Revue : trimestrielle

Ce tableau de bord répond aux questions de la clause 9.1 : quoi mesurer, comment, quand, qui mesure, quand analyser et qui analyse. Les valeurs de départ correspondent à la situation d'octobre 2026, avant la mise en œuvre du plan de traitement.

| Id | Indicateur | Formule | Valeur de départ | Cible | Fréquence | Source | Responsable | Objectif |
|---|---|---|---|---|---|---|---|---|
| KPI-01 | Avancement des mesures prioritaires | Mesures P1 réalisées / mesures P1 | 0 / 12 | 12 / 12 au 31/03/2027 | Mensuelle | Plan d'action, CISO Assistant | RSSI | O1 |
| KPI-02 | Risques résiduels élevés | Nombre de risques au niveau élevé | 5 | 0 | Trimestrielle | Analyse de risques AR_01 | RSSI | O1 |
| KPI-03 | Couverture MFA des comptes à privilèges | Comptes à privilèges avec MFA / comptes à privilèges | Non mesuré | 100 % | Mensuelle | Annuaire et console AWS | DSI | O2 |
| KPI-04 | Taux de clic au phishing | Clics / courriels de simulation envoyés | Non mesuré | moins de 5 % | Trimestrielle | Outil de simulation | RSSI | O3 |
| KPI-05 | Tests de restauration réussis | Tests réussis en moins de 4 h / tests réalisés | 0 test | 4 par an, 100 % réussis | Trimestrielle | Rapports de test | DSI | O4 |
| KPI-06 | Notification des incidents majeurs dans les délais | Incidents notifiés à temps / incidents majeurs | Pas de procédure | 100 % | À chaque incident | Registre des incidents | RSSI | O5 |
| KPI-07 | Contrats critiques conformes à DORA | Contrats avec clauses de l'article 30 / contrats critiques | 0 / 5 | 5 / 5 | Trimestrielle | Registre d'information des prestataires | Achats | O6 |
| KPI-08 | Revues des habilitations réalisées | Revues réalisées / revues prévues | 0 / 4 | 4 / 4 par an | Trimestrielle | Comptes rendus de revue | RSSI | O7 |
| KPI-09 | Délai de déclaration Tracfin | Jours entre l'alerte et la déclaration (moyenne) | Non mesuré | moins de 30 jours | Mensuelle | Outil LCB-FT | Conformité | O8 |
| KPI-10 | Couverture EDR | Postes et serveurs avec EDR / total | 0 % | 100 % | Mensuelle | Console EDR | RSSI | O1 |
| KPI-11 | Contrôles de l'Annexe A en place | Contrôles conformes / contrôles applicables | 0 / 90 | En hausse à chaque trimestre | Trimestrielle | SoA, CISO Assistant | RSSI | O1 |
| KPI-12 | Non-conformités ouvertes depuis plus de 90 jours | Nombre | 0 | 0 | Mensuelle | [Registre des non-conformités](08-amelioration.md) | RSSI | Clause 10 |

**Analyse et restitution**

- Le RSSI collecte les valeurs et les analyse chaque mois.
- Un tableau de bord est présenté chaque trimestre en comité sécurité, puis au COMEX.
- Un indicateur hors cible pendant deux périodes de suite donne lieu à une action corrective dans le [registre](08-amelioration.md).
- Les tendances de l'année sont un élément d'entrée de la [revue de direction](07-revue-de-direction.md).
