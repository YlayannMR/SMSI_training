# Audit interne (clause 9.2)

Document : SMSI-06 · Version 1.0 · Propriétaire : Responsable de l'audit interne · Revue : annuelle

## Programme d'audit sur trois ans

L'audit interne vérifie que le SMSI respecte les exigences d'Orséa et de la norme ISO 27001, et qu'il est appliqué efficacement. Il est réalisé par l'audit interne de la banque ou par un cabinet externe : jamais par le RSSI, qui ne peut pas auditer son propre travail.

| Année | Périmètre audité | Période | Auditeur |
|---|---|---|---|
| 2027 | Clauses 4 à 10, contrôles 5.15 à 5.23 (accès et prestataires), 8.13 (sauvegardes) | Juin 2027 | Cabinet externe |
| 2028 | Clauses 4 à 10, contrôles 5.24 à 5.30 (incidents, continuité), 8.7 à 8.16 (exploitation) | Juin 2028 | Audit interne |
| 2029 | Clauses 4 à 10, contrôles 6.x (personnes), 7.x (physique), 8.25 à 8.33 (développement) | Juin 2029 | Audit interne |

Les clauses 4 à 10 sont auditées chaque année. Les contrôles de l'Annexe A sont répartis sur trois ans, en commençant par ceux liés aux risques les plus élevés.

**Méthode** : entretiens, revue documentaire, échantillonnage (comptes, contrats, journaux), observation. Critères : ISO 27001:2022, PSSI d'Orséa, DORA. Les résultats sont présentés à la direction et les écarts sont suivis dans le [registre des non-conformités](08-amelioration.md).

## Pré-audit du 19 octobre 2026

Avant le premier audit officiel, un audit à blanc a été réalisé pour mesurer l'écart de départ.

- **Périmètre** : clauses 4 à 10, SoA, analyse de risques, contrats des prestataires critiques
- **Méthode** : revue documentaire et revue de l'étude EBIOS RM dans CISO Assistant
- **Auditeur** : analyste GRC (pré-audit seulement ; l'audit officiel sera indépendant)

**Points forts**

- Analyse de risques EBIOS RM complète sur les cinq ateliers, avec des justifications argumentées
- Déclaration d'applicabilité qui couvre les 93 contrôles, exclusions justifiées
- Plan de traitement chiffré, priorisé, avec un responsable par mesure

**Constats**

| Id | Type | Exigence | Constat |
|---|---|---|---|
| NC-01 | Non-conformité mineure | 5.2 | La PSSI existe en version 0.1 mais n'a pas encore été approuvée par la direction ni diffusée. |
| NC-02 | Non-conformité majeure | 6.1.3 f | Les risques résiduels n'ont pas été acceptés formellement par leurs propriétaires. |
| NC-03 | Non-conformité majeure | Annexe A 5.20, DORA art. 30 | Les contrats des 5 prestataires TIC critiques ne contiennent pas les clauses minimales exigées. |
| NC-04 | Non-conformité mineure | 7.2 | Aucune preuve de compétence n'est demandée au prestataire de support pour ses agents. |
| NC-05 | Non-conformité mineure | 6.1.2 | Incohérence dans l'analyse de risques : l'action d'exploitation du scénario CA_06 reprend celle de CA_05, et un couple source de risque / objectif retenu n'est utilisé par aucun scénario. |
| NC-06 | Non-conformité mineure | 7.5 | La SoA et le plan de traitement n'ont ni numéro de version ni approbation. |
| OBS-01 | Observation | 9.1 | Les indicateurs sont définis mais la plupart ne sont pas encore mesurés. |
| OBS-02 | Observation | 5.3 | Dans l'outil GRC, aucune mesure n'est encore assignée nominativement à une personne. |

**Conclusion** : le SMSI est bien conçu mais pas encore en fonctionnement. Les deux non-conformités majeures (NC-02, NC-03) bloqueraient une certification et doivent être levées avant l'audit de juin 2027.
