# Contexte pour le rapport de stage ENSAE — Document 1/2
# Mission IGF « Stratégie d'achat en matière de déplacements professionnels » (février–juin 2026)

## 0. Mode d'emploi (à l'attention du LLM rédacteur)

Ce document est une **source de contexte**, pas un texte à reproduire. Il décrit la première des deux missions du stage de fin d'études ENSAE (3A) effectué à l'Inspection générale des finances (IGF). La seconde mission, « revue de dépenses primes et indemnités », fait l'objet du document 2/2.

Le rapport ENSAE attendu fait environ 30 pages. Il comprend une introduction, un développement (problème, données, méthodes, résultats critiqués), une conclusion, une bibliographie, des annexes et deux notes de synthèse (FR et EN). La grille valorise le lien avec les enseignements de l'ENSAE, la fidélité à la démarche réellement suivie, la part des tiers et la prise de recul.

Règles :

- **Ne jamais inventer de chiffres.** Les chiffres ci-dessous proviennent de la note finale de la mission (juin 2026) ou des travaux du stagiaire.
- `[À COMPLÉTER]` signale une information manquante et `[À CONFIRMER]` une information probable mais non vérifiée.
- **Confidentialité : la note IGF porte la mention « NOTE CONFIDENTIELLE ».** Le rapport ENSAE devra très probablement être déclaré confidentiel (fichier `NOM_Prénom_3A25_CONF.pdf`, mention sur la page de garde). À valider avec le maître de stage. `[À CONFIRMER]`
- Ne pas recopier la note IGF : reformuler et centrer le propos sur **le travail du stagiaire** (données, méthodes, outils), la note servant de source de résultats.

---

## 1. Fiche d'identité de la mission

| Élément | Contenu |
|---|---|
| Intitulé | Stratégie d'achat en matière de déplacements professionnels : retour d'expérience en matière de maîtrise de la dépense et de simplification pour les agents |
| Commanditaire | Ministre de l'action et des comptes publics (lettre de mission du 26 février 2026, adressée à la cheffe du service de l'IGF) |
| Livrable | Note confidentielle n° 2026-E-028-02 du 11 juin 2026 (≈ 120 pages avec les annexes), restitution orale le 5 juin 2026 |
| Équipe | Valérie Champagne, inspectrice générale des finances (supervision) ; François-Xavier Boell, inspecteur des finances ; Paco Goze, inspecteur stagiaire des finances (le stagiaire, cosignataire de la note) |
| Maître de stage | `[À COMPLÉTER]` |
| Structure du livrable | Note de synthèse (3 propositions) ; annexe I (modalités d'achat) ; annexe II (atteinte des objectifs de réduction et de verdissement) ; **annexe III (méthodes d'analyse des ordres de mission et des frais associés)** ; annexe IV (personnes rencontrées) ; présentation de restitution ; lettre de mission |

**Rôle du stagiaire** : prise en charge des travaux quantitatifs, à savoir l'exploitation des extractions Chorus DT, le calcul des indicateurs, les graphiques, la rédaction de commentaires et de passages méthodologiques. Les méthodes de l'annexe III correspondent aux traitements développés par le stagiaire `[À CONFIRMER : périmètre exact de sa contribution, notamment sur l'analyse de la dépense DAE et les annexes I et II]`.

---

## 2. Le problème posé

### 2.1 Contexte institutionnel

- La **circulaire du Premier ministre n° 6425/SG du 21 novembre 2023** (transformation écologique de l'État) fixe des cibles de réduction et de verdissement des déplacements. Elle prévoit une baisse de la dépense de déplacements professionnels de **–20 % en 2024 et –30 % en 2027 par rapport à 2019**. Elle prévoit aussi une baisse des trajets aller en avion de –20 % en 2024 et –30 % en 2027. L'avion n'est autorisé qu'en l'absence d'alternative ferroviaire de moins de 4 heures.
- Une **stratégie interministérielle d'achat** (portée par la direction des achats de l'État, DAE) pousse à recourir aux **agences de voyage** titulaires de marchés. Les enjeux sont les remises commerciales négociées, la dématérialisation et le respect de la politique de consommation.
- Constat déclencheur : la dépense de déplacements suivie par la DAE est passée de **1,1 à 1,5 Md€ entre 2019 et 2025 (+40 %)**, alors que l'objectif était de la réduire.

### 2.2 Les trois axes de la commande

1. Analyser la dynamique de la dépense, avec un périmètre pertinent, les facteurs d'évolution et la distinction entre effets prix et effets volume.
2. Se prononcer sur l'atteinte des objectifs de réduction et de verdissement, et sur la pertinence des indicateurs retenus.
3. Apprécier la qualité de service des agences de voyage et le parcours utilisateur des agents.

### 2.3 Reformulation « question scientifique » (utile pour l'introduction ENSAE)

> La dépense est-elle un bon indicateur de l'évolution des déplacements ? Si non, comment mesurer à partir de données de gestion (ordres de mission, états de frais) le volume, la durée, la distance et le mode des déplacements ? Comment caractériser les comportements d'achat des agents (agence vs achat direct) ?

La réponse de la mission est que la dépense est un mauvais indicateur, parce qu'elle dépend des conventions de périmètre et des effets prix. Il faut lui préférer des **données physiques** tirées des ordres de mission. C'est ce basculement qui justifie tout le travail d'ingénierie de la donnée du stagiaire.

---

## 3. Notions métier

- **Déplacement temporaire** : déplacement hors résidence familiale et administrative, couvert par un **ordre de mission (OM)**. Les trajets domicile-travail sont exclus.
- **OM** : identifié par un numéro unique. Il précise le missionné, l'objet, le lieu de départ (résidence administrative ou familiale), la destination, les dates et les modalités de transport. Les OM ont des statuts (« Traité », « Validé », « Sans frais »). Il existe des **OM permanents** et des OM de **formation initiale**, qui ont pu être de très longue durée (> 300 jours).
- **État de frais (EF)** : rattaché à un OM, il récapitule les remboursements au missionné par nature de frais (repas, hébergement, train et avion payés par le missionné, indemnités kilométriques…). Statut retenu : « C1 – Payé par Chorus ».
- **Demandes de paiement / prestations d'agence** : paiements à l'agence de voyage par type de prestation, codés **FAV** (avion), **FHO** (hôtel), **FTR** (train), **FVL** (location de voiture), **FDI** (divers), **ZFE** (frais d'agence, soit la rémunération de l'intermédiaire).
- **Indemnité de nuitée** : remboursement **forfaitaire** de l'hébergement. Le missionné garde la différence si la nuit coûte moins cher. Le remboursement au réel représente moins de 1 % du total.
- **Réservation en ligne / hors ligne** : en ligne, le missionné choisit sur l'outil (Chorus DT) ; hors ligne, l'agence construit l'offre à la demande. Les frais d'agence sont plus élevés hors ligne.
- **Applications** : **Chorus** (comptabilité de l'État), **Chorus DT** (gestion des déplacements, pilotée par l'**AIFE**), ainsi que d'autres outils (FD@ligne, Chorege…). Aucune base consolidée n'existe pour tout l'État.
- **Périmètre « SG MEF »** : agents des ministères économiques et financiers **hors DGFiP, DGDDI et Insee**.

---

## 4. Les données

### 4.1 Trois sources

| Source | Contenu | Usage |
|---|---|---|
| **DAE** (consolidation à partir de Chorus) | Dépenses de déplacements par ministère et programme budgétaire, 2019–2025 | Analyse de la dépense et construction d'un périmètre restreint |
| **AIFE** (extractions Chorus DT) | Récapitulatif des OM (n°, service, date de début, lieu de départ, destination, enveloppe, centre de coût) ; EF (n°, OM de référence, statut, type de frais, montant, dates) ; prestations d'agence ; **table de jointure OM ↔ matricule agent** ; indemnités kilométriques par service et barème | Volumes, durées, nombre de missionnés, concentration, indemnités kilométriques. Périmètre : services utilisant Chorus DT de façon constante sur 2019–2025 (MAASA, Culture, MTE, DGAC, Insee, DGFiP) |
| **SG MEF** (extractions Chorus DT) | OM, EF et prestations d'agence du périmètre SG MEF | Distances, modes de transport, canal d'achat, part des agences |

### 4.2 Fichiers manipulés par le stagiaire (noms réels)

- Fichier « global » multi-feuilles (OM, EF).
- `DGFiP/2026_04_01_IGF_EF_DONNES_PHYSIQUES_DGFIP_{ANNEE}.xlsx` : EF de la DGFiP, un fichier par an.
- `OM données physiques/2026_04_01_IGF_OM_DONNEES_PHYSIQUES_{ANNEE}.xlsx` (2019–2026) : OM avec dates, lieux et codes résidence.
- `2026_IGF_PRESTATION.xlsx` : prestations d'agence **sans date**.
- `NB_OM_HEAD.xlsx` : groupe de société, matricule, n° d'OM, date.

**Volumétrie** : plusieurs centaines de milliers de lignes par fichier, jusqu'à 532 000 OM traités par an sur le périmètre AIFE. La colonne « Année » d'un fichier comptait à elle seule **844 247 valeurs manquantes**. Ces fichiers sont trop lourds pour Excel, d'où le passage à Python.

### 4.3 Limites des données (reprises dans l'annexe III)

- **Données partielles** : seule une partie des services de l'État utilise Chorus DT. Les résultats valent pour le périmètre étudié, pas pour l'État entier.
- **Destinations non géocodables dans les données AIFE** : les codages sont hétérogènes (nom de ville, code aéroport, code commune Insee, codes non identifiés) et aucune table de correspondance n'existe. Le calcul des distances a donc été fait uniquement sur les données SG MEF.
- **Jointure partielle prestations ↔ OM** : des prestations d'agence ont des n° d'OM introuvables dans le récapitulatif des OM. Or la date n'est présente que dans ce récapitulatif, ce qui rend impossible l'analyse temporelle sur ces lignes. Les analyses de canal d'achat ont donc été basculées sur les données SG MEF.
- **Granularité** : plusieurs lignes par OM dans les EF, d'où un risque de double comptage.
- **Valeurs manquantes corrélées** (« Année » et « Nombre de jours » vides sur les mêmes lignes).
- **Saisie libre des villes** : fautes, régions ou listes de départements à la place d'une ville, mentions du type « DIVERS NOVEMBRE », homonymies entre petites communes françaises et villes étrangères.
- **OM permanents et formations initiales non neutralisés** : ils rehaussent mécaniquement la durée moyenne, sans remettre en cause la tendance à la baisse.
- **Nomenclatures hétérogènes** entre fichiers (codes de type de frais, libellés de statut).

---

## 5. Chantiers quantitatifs : méthodes et résultats

Démarche générale : premières explorations sous **Excel** (Power Query, tableaux croisés dynamiques, `SOMME.SI`/`NB.SI`), puis bascule vers **Python** (pandas, NumPy, openpyxl, matplotlib, requests). Ce passage répondait à trois besoins : la volumétrie, la **reproductibilité** (méthodes réapplicables à d'autres services, recommandation n° 1) et la traçabilité des choix. Les scripts produisent des classeurs Excel structurés, avec des onglets de résultats et des onglets de contrôle. Les méthodes ont été rédigées sous forme de pas-à-pas dans l'annexe III pour être reprises par d'autres administrations, y compris celles qui utilisent d'autres logiciels que Chorus DT.

### 5.1 La dépense n'est pas un bon indicateur (travail sur les données DAE)

- La DAE consolide trois catégories : fonctionnement des véhicules, investissement dans les véhicules et « autres dépenses de déplacement ». La mission se limite à la troisième et exclut le parc automobile.
- **Dépense DAE (M€)** : 1 063 (2019), 964 (2021), 1 191 (2022), 1 335 (2023), 1 757 (2024, pic lié notamment aux Jeux olympiques et à la Nouvelle-Calédonie), 1 490 (2025), soit **+40 %**. Les ministères de l'Intérieur et des Armées représentent plus de 70 % de la dépense en 2025. En base 100 en 2019, l'Intérieur est à 238 en 2025 (351 en 2024) et les Armées à 122. Les ministères économiques et financiers, l'agriculture et la culture sont en baisse.
- **Construction d'un périmètre restreint « pilotable »**, en lien avec la DAE. Sont exclus les programmes P178 (forces), P347 (G7), P152 (gendarmerie), P176 (police) et P161 (sécurité civile), ainsi que les marchés associés (hébergement collectif des CRS, avions Beechcraft, locations courte durée). Certains éléments n'ont pas pu être exclus faute de temps : compensation du tarif militaire hors P178, éloignements forcés, congés bonifiés et mutations.
- **Dépense restreinte (M€)** : 516 (2019), 377, 494, 566, 592, 571 (2025), soit **+10 %** au lieu de +40 %.
- **Effets prix** : l'indice des prix du transport aérien (DGAC) passe de 68,4 (janvier 2019) à 96,8 (décembre 2025), soit +42 %. Plusieurs indemnités ont été revalorisées : les indemnités kilométriques en 2022, les indemnités de repas et d'hébergement en 2023.
- **Conclusion méthodologique** : la mesure par la dépense dépend d'un choix de périmètre conventionnel et d'effets prix exogènes. Il faut passer aux **données physiques**.

Ce chantier inclut les travaux de « suivi budgétaire / périmètre de dépenses DAE » menés par le stagiaire `[À CONFIRMER : part exacte du stagiaire]`.

### 5.2 Nombre et durée des déplacements (données AIFE — scripts `analyse_missions.py` et `compute_day_per_OM_DGFiP.py`)

**Méthode finale (annexe III)** :

1. Sélection des EF au statut « C1 – Payé par Chorus » (ou « C1 »).
2. Sélection des EF de **repas**. L'hypothèse est qu'une mission de plus d'une journée génère nécessairement des frais de repas, ce qui en fait un marqueur fiable de l'existence du déplacement.
3. **Dédoublonnage : un seul EF par OM** (`drop_duplicates(subset=["OM de référence"])`).
4. **Année dérivée de la date de début de mission**, et non de la colonne « Année » lacunaire.
5. **Durée = date de fin – date de début + 1**, plutôt que la somme d'une colonne « Nombre de jours », qui double-comptait.
6. Par année : somme des durées (nombre total de jours), moyenne, médiane, et répartition en 1, 2, 3, 4, 5 jours et plus d'une semaine.

**Itérations de mise au point**, à valoriser comme démarche et comme contrôles de cohérence :

- Premières versions fausses par double comptage, repérées grâce aux ordres de grandeur.
- Filtrage prématuré des années manquantes, qui faisait perdre des OM.
- Catégorie « 0 jour / aller-retour » ajoutée parce que les pourcentages ne sommaient pas à 100 %. Elle a ensuite été rendue inutile par la convention « +1 ».
- Seuil de troncature à 90 jours testé puis abandonné dans la version finale : les OM longs ont été conservés et signalés `[À CONFIRMER]`.
- Histogramme des durées à classes de largeur variable (1 jour jusqu'à 30, puis 5 jours jusqu'à 90, puis 30 jours) sur échelle log, pour visualiser la queue de distribution (OM permanents, formations).

**Résultats (périmètre AIFE : MAASA, Culture, MTE, DGAC, Insee, DGFiP)** :

| Indicateur | 2019 | Point bas | 2025 |
|---|---|---|---|
| OM traités (milliers) | 532 | 329 (2021) | 432 |
| Jours de mission (millions) | 4,4 | 3,3 (2021) | 3,0 (soit **–31 %**) |
| Missionnés (milliers) | 94 | 71 (2021) | 86 |
| Durée moyenne (jours) | 13,3 | — (17,3 en 2020) | 11,4 |
| Durée médiane (jours) | 3 | — (5 en 2020) | 2 |
| Déplacements moyens par missionné | 5,67 | 4,00 (2020) | 5,04 |

Lecture : il y a moins de missionnés, qui se déplacent moins longtemps et moins souvent. La moyenne est tirée vers le haut par les OM permanents et les formations initiales, non neutralisés, ce qui explique l'écart entre moyenne et médiane.

### 5.3 Nombre de missionnés et concentration des déplacements (script `build_excel.py`)

**Méthode** : grâce à la table de jointure OM ↔ matricule, on compte les OM par matricule et par année. On décrit ensuite la distribution : moyenne, médiane, écart-type, déciles D1–D9, D99, courbe de Lorenz, **indice de Gini**, part des OM captée par le top 10 % et le top 1 %, part des agents ayant moins de 4, moins de 6, plus de 12 et plus de 24 OM. Les résultats sont déclinés au global et par groupe de société, dans un classeur à une feuille par groupe.

**Typologie conventionnelle retenue par la mission** :

- Les **voyageurs occasionnels** font moins de 4 déplacements par an. Ils représentent **plus de la moitié** des agents s'étant déplacés au moins une fois : 52,3 % en 2019, 63,2 % en 2020, 56,2 % en 2025.
- Les **grands voyageurs** font plus de 12 déplacements par an. Ils représentent **11 à 15 %** de ces agents : 14,7 % en 2019, 5,9 % en 2020, 11,3 % en 2025.
- Biais signalé : les agents sédentaires (0 OM) ne figurent pas dans la table, ce qui surreprésente les grands voyageurs dans la population totale.

Valeurs du Gini et parts du top 10 % : `[À COMPLÉTER depuis le classeur analyse_OM_concentration.xlsx]`.

**Usage dans la note** : cette hétérogénéité fonde la recommandation de différencier le parcours utilisateur selon le profil (simplifier la validation des OM et ouvrir l'accès à la réservation en ligne pour les grands voyageurs).

### 5.4 Distances parcourues et types de destination (données SG MEF — script `calculer_deplacements.py`)

**Méthode** :

1. Sélection des OM au statut « Traité ».
2. Ville de départ = résidence administrative ou familiale selon le champ de l'OM. S'il y a plusieurs villes dans un champ, seule la première est retenue.
3. **Géocodage avec Nominatim (OpenStreetMap)**, à une requête par seconde. La stratégie se fait **en deux passes** pour lever les homonymies : recherche d'abord en France, puis recherche mondiale si rien n'est trouvé. Les villes sont étiquetées FR, DROM-COM (au-delà de 1 500 km de Paris pour un résultat français) ou ÉTRANGER.
4. **Distance à vol d'oiseau par la formule de Haversine**, calculée localement. Une première piste de distance routière via le service OSRM a été abandonnée : elle créait une dépendance réseau, était lente et ne s'appliquait pas à l'international.
5. **Imputation par la médiane** des distances pour les villes non reconnues.
6. Un OM vaut un aller-retour, d'où **distance totale = somme × 2**.
7. **Classification** des déplacements par croisement des classes de départ et de destination : métropole, outre-mer ou étranger. Un trajet entre deux villes d'outre-mer est compté comme « métropole », et seuls les trajets métropole ↔ outre-mer sont comptés « outre-mer ».

**Ingénierie annexe** :

- **Cache JSON persistant** des géocodages, pour ne pas réinterroger l'API à chaque exécution.
- Normalisation automatique d'anciens libellés du cache. Un bug a été diagnostiqué : le renommage « FR/DOM-TOM » en « FR/DROM » faisait tomber des lignes en « Inconnu ».
- **Onglet de contrôle des distances supérieures à 250 km**, avec lien cartographique et colonne de correction manuelle prioritaire `[À CONFIRMER : mise en œuvre effective]`.

**Résultats (SG MEF)** :

- OM traités : **76 000 (2019), 48 000 (2021), 71 000 (2025)**.
- Distances : environ 71 millions de km en 2019 (36 en métropole, 24 vers l'outre-mer, 11 à l'étranger) contre environ 57 millions en 2025 (32, 21 et 4), soit **–20 %**.
- La baisse s'explique surtout par l'étranger. La part des OM à l'étranger passe de **2,3 % à 1,4 %** et leur part dans les kilomètres de **15,5 % à 6,4 %**. Les distances en métropole et en outre-mer sont stables.

### 5.5 Modes de transport et report modal (données SG MEF)

**Méthode** : nombre de billets de train = nombre de prestations d'agence FTR + nombre d'EF « Train (payé par missionné) ». Même calcul pour l'avion (FAV + EF « Avion »). Le ratio train/avion sert d'indicateur de report modal.

**Données** (nombre de billets) :

| Année | Avion total | dont agence | dont agent | Train total | dont agence | dont agent | Voiture | dont véhicule personnel |
|---|---|---|---|---|---|---|---|---|
| 2019 | 3 596 | 3 141 | 455 | 16 296 | 10 716 | 5 580 | 10 764 | 10 079 |
| 2020 | 1 177 | 979 | 198 | 5 421 | 2 927 | 2 494 | 5 895 | 5 581 |
| 2021 | 1 463 | 1 191 | 272 | 6 779 | 3 625 | 3 154 | 7 984 | 7 591 |
| 2022 | 2 817 | 2 364 | 453 | 12 821 | 8 360 | 4 461 | 8 845 | 8 300 |
| 2023 | 3 158 | 2 605 | 553 | 17 286 | 12 236 | 5 050 | 10 105 | 9 603 |
| 2024 | 2 924 | 2 384 | 540 | 18 645 | 13 008 | 5 637 | 10 346 | 9 907 |
| 2025 | 2 650 | 2 169 | 481 | 13 288 | 7 441 | 5 847 | 9 223 | 8 792 |

**Résultats** :

- En base 100 en 2019, l'avion tombe à 74 en 2025, soit **–26 %**, en ligne avec l'objectif de la circulaire. Le train atteint un pic à 114 en 2024 puis revient à 82 en 2025.
- Le rapport train/avion est stable autour de 4,5 entre 2019 et 2022, monte à **6,4 en 2024** puis revient à **5,0 en 2025**. C'est un indice de report modal.

### 5.6 Canal d'achat : agence vs achat direct (données SG MEF ; jointure `enrichir_prestation_v3.py`)

**Méthode** :

- Construction de catégories de dépenses à partir des libellés de types de frais. Les repas regroupent les libellés contenant « repas », « déjeuner » ou « dîner ». L'hébergement regroupe « nuitée », « hébergement » et « hôtel ». Viennent ensuite l'avion, le train, les indemnités kilométriques, les autres transports et une catégorie divers.
- Agrégation des prestations d'agence par code (FAV, FHO, FTR, FVL, FDI, ZFE).
- Calcul de ratios : frais d'agence (ZFE) sur total versé à l'agence ; prestations d'agence sur (agence + remboursements aux missionnés) ; parts agence / missionné par poste (hébergement, avion, train), en montant et en nombre de billets.
- **Ventilation des billets de train 2025 par tranche de prix** : moins de 30 €, 30–50, 50–100, 100–200, 200–300, plus de 300 €.
- **Jointure prestations ↔ OM** sur « N° de l'OM » pour dater les prestations (concaténation des 7 fichiers annuels d'OM, puis jointure gauche). Des onglets de contrôle recensent les OM non retrouvés, ventilés par groupe de société, par nature de dépense et en croisement. Ce diagnostic a conduit à constater le recoupement partiel des données AIFE. Taux d'appariement : `[À COMPLÉTER]`.

**Résultats (SG MEF)** :

- **Part des prestations d'agence dans le coût total** : entre **13 et 18 %** hors années Covid, et 13 % en 2025. Plus de 80 % du coût correspond donc à des remboursements aux missionnés.
- **Structure des dépenses 2025** : hébergement remboursé 49 %, repas 27 %, prestations d'agence 13 %, transport remboursé 8 %, divers 3 %. Repas et hébergement remboursés représentent environ **les trois quarts** (76 %).
- **Hébergement** : **98 à 99 %** de la dépense est payée aux missionnés. L'explication avancée est le forfait de nuitée. Un contrôle du SG MEF sur 445 EF du premier trimestre 2026 montre que, dans **86 %** des cas, la facture est inférieure à l'indemnité versée.
- **Avion** : l'agence représente **91 à 95 %** de la dépense, et la part payée par les missionnés passe de 5 % en 2019 à 9 % en 2025. L'agence évite aux agents d'avancer des sommes élevées.
- **Train** : en montant, l'agence passe de 75 % à 66 % entre 2019 et 2025. En nombre de billets, elle passe de 66 % à 56 %. Les billets achetés directement sont donc en moyenne moins chers. Par tranche de prix en 2025 : **83 % des billets de moins de 30 € sont achetés par les missionnés**, alors que l'agence représente 81 % des billets entre 200 et 300 € et 74 % au-delà de 300 €. Titre de graphique retenu : « Les billets coûteux passent davantage par les agences ». Ce comportement est jugé rationnel, pour l'agent comme pour l'État, parce que les frais d'agence sont forfaitaires quel que soit le prix du billet.
- **Frais d'agence (ZFE) sur total versé à l'agence** : 1,9 % (2019), 1,7, 1,4, 1,2, 1,0, 0,8, 0,9 % (2025). C'est cohérent avec les chiffres transmis par l'agence Globéo Travel (1,9 % en 2019, 1,0 % en 2025), une **validation externe** de la méthode.

### 5.7 Indemnités kilométriques (données AIFE)

- **Méthode** : sélection des EF traités par Chorus, puis des barèmes « IK Standard » et « SNCF 2e classe », puis somme par service du champ « Quantité » (kilomètres indemnisés). Le périmètre est plus large (inclut Justice, Intérieur et ministères sociaux).
- **Résultat** : les kilomètres indemnisés ont davantage baissé à la DGFiP que dans les autres services, en base 100 en 2019 `[À COMPLÉTER : valeurs exactes]`. Cela illustre la politique DGFiP 2026 de renouvellement de la flotte en véhicules électriques et d'assouplissement de l'usage des véhicules de service.

### 5.8 Travaux auxquels le stagiaire n'est pas l'auteur principal (à distinguer dans la « part des tiers »)

- **Comparaison de prix** Chorus DT / prix publics, réalisée par le SG MEF à la demande de la mission les 13 et 14 avril 2026. Elle porte sur les 10 trajets ferroviaires et les 10 trajets aériens aux plus gros montants, avec une nuit d'hôtel. Résultats : prix du train identiques ; prix de l'avion inférieurs ou égaux sauf Paris–Cayenne ; hôtels inférieurs ou égaux sauf 3 destinations sur 18.
- **Gains des accords commerciaux** (données DAE) : remises Air France de 6,9 % et SNCF de 7,4 % en 2024, gain de 18,7 % sur les tarifs négociés Accor en 2025.
- **Entretiens qualitatifs** avec les responsables achat, l'AIFE, la DAE, la DGFiP, des universités, l'AMUE, des cabinets, etc. `[À CONFIRMER : participation du stagiaire]`.

---

## 6. Du chiffre à la recommandation

**Messages de la note** :

1. Le périmètre de dépenses suivi ne permet pas d'apprécier l'évolution des déplacements.
2. D'après les OM étudiés, les engagements de réduction et de verdissement sont respectés.
3. Le recours à l'agence est pertinent : il a un coût limité, il automatise la gestion, il encadre la consommation et il donne accès aux remises.
4. Il faut convaincre les agents de l'utilité des agences.
5. Il faut laisser aux services la gestion des déplacements dans un cadre interministériel fixé à grandes lignes.

**Propositions** :

- **n° 1** : étendre les méthodes d'analyse développées, c'est-à-dire le travail du stagiaire, à un champ plus large, y compris les universités.
- **n° 2** : consacrer des ressources des missions ministérielles d'achat au suivi de l'exécution des marchés d'agence.
- **n° 3** : dans la future circulaire, fixer des cibles sur des **indicateurs pilotables** (nombre de missions, distances) plutôt que sur la dépense.

Le lien avec le travail quantitatif est direct. La proposition n° 3 découle de la démonstration que la dépense est un mauvais indicateur et que les indicateurs physiques sont calculables. La proposition n° 1 repose sur la réplicabilité des pipelines. Les recommandations sur le parcours des grands voyageurs reposent sur l'analyse de concentration.

**Principes de rédaction appliqués par le stagiaire** : titres de graphiques qui énoncent le constat ; commentaires au service d'un argument ; hypothèses explicitement signalées (par exemple l'effet du forfait de nuitée) ; notes méthodologiques sur les limites (OM permanents, périmètre partiel).

---

## 7. Visualisation : charte graphique IGF

Les principes ont été appliqués aux graphiques produits sous matplotlib puis Excel :

- Le titre énonce le message.
- Palette de verts, gris pour « Autres », orange pour faire ressortir une valeur.
- Barres plutôt que camemberts ; donut pour mettre en valeur un chiffre unique.
- Étiquettes plutôt qu'axe vertical.
- Au plus 5 séries par graphique ; base 100 pour comparer des évolutions ; valeurs ordonnées.
- Note de lecture et source (« Mission d'après données du SG MEF / de l'AIFE / de la DAE »).

---

## 8. Outils

- **Python** : pandas (lecture multi-feuilles, concaténation, filtres, `drop_duplicates`, `merge`, `groupby`), NumPy (quantiles, Gini, Lorenz), openpyxl (classeurs formatés, onglets de contrôle, `ExcelWriter` en mode ajout avec `if_sheet_exists="overlay"`), matplotlib, requests (API Nominatim), `math` (Haversine), JSON (cache).
- **Excel** : Power Query, tableaux croisés dynamiques, `SOMME.SI` / `NB.SI`.
- **Systèmes de l'État** : Chorus, Chorus DT (sources des extractions AIFE et SG MEF).
- **Assistant IA (LLM)** utilisé pour écrire et déboguer des scripts et pour des reformulations (voir § 11).

---

## 9. Correspondance avec les attendus ENSAE

| Attendu | Illustration |
|---|---|
| S'intégrer, s'approprier outils et données | Notions OM / EF / prestations, nomenclatures Chorus DT, codes de prestations, statuts |
| Poser une question scientifique adaptée | Passer de « la dépense a-t-elle baissé ? » à « comment mesurer les déplacements indépendamment des effets prix et de périmètre ? » |
| Mobiliser les enseignements ENSAE | Économétrie et statistique appliquée (qualité des données, biais de sélection, choix de périmètre, effets prix vs volume, indices base 100), statistique descriptive (quantiles, Lorenz, Gini), data engineering (jointures, dédoublonnage, pipelines reproductibles), géocodage et distance géodésique, imputation, visualisation |
| Proposer et mettre en œuvre une solution | Pipelines Python documentés, réplicables sur d'autres logiciels (annexe III) |
| Analyser et critiquer | Limites de périmètre, OM permanents, vol d'oiseau, imputation médiane, jointures partielles, hypothèses comportementales non testées ; validation croisée avec Globéo Travel |
| Restituer | Graphiques charte IGF, rédaction de passages de la note, présentation de restitution |

---

## 10. Limites et recul critique

- **Représentativité** : environ 4 ministères sur Chorus DT, et le seul SG MEF pour les distances et les canaux d'achat. L'extrapolation à l'État est impossible, d'où la proposition n° 1.
- **Causalité non établie** : la baisse de l'avion coïncide avec la circulaire de 2023 mais aussi avec l'après-Covid (télétravail, visioconférence). Le lien entre le forfait de nuitée et la préférence pour l'hôtel réservé soi-même reste une hypothèse, partiellement étayée par le contrôle sur 445 EF.
- **Mesure** : la distance à vol d'oiseau sous-estime les trajets ; l'imputation par la médiane écrase la variance ; retenir seulement la première ville ignore les missions multi-étapes ; le proxy « EF repas » exclut les missions sans frais de repas.
- **Périmètre** : OM permanents et formations non neutralisés ; en conséquence, la durée moyenne est à interpréter avec prudence et la médiane est plus robuste.
- **Contrainte de temps** : environ 3,5 mois entre la lettre de mission et la note, ce qui explique plusieurs neutralisations non réalisées.
- **Pistes** : référentiel de communes (code Insee) pour le géocodage, distances réseau, neutralisation des OM permanents, table de correspondance des destinations AIFE, extension aux universités et aux autres logiciels, analyse des coûts unitaires par canal, sondages auprès des agents.

---

## 11. Points à compléter / trancher par l'auteur

- Dates exactes du stage, maître de stage, référent ENSAE.
- Contribution exacte du stagiaire par annexe et part du travail des deux inspecteurs.
- Valeurs de Gini et de concentration, taux d'appariement de la jointure, nombre de villes géocodées et non reconnues, nombre de corrections manuelles.
- Statut confidentiel du rapport ENSAE et éventuel masquage de chiffres.
- **Part des tiers** : encadrement (cadrage des indicateurs, validation des conventions), apports du SG MEF, de l'AIFE et de la DAE (extractions, comparaison de prix), et **usage d'un assistant IA** pour le code. À présenter honnêtement en soulignant ce qui relève du stagiaire : règles métier, diagnostic des erreurs, choix méthodologiques, validation.
