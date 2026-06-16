# 🚀 VivaTech 2026 — Programme de Valorisation & Commercialisation
## 📅 Guide Stratégique pour Louis & Alban Hauseux (17–18 Juin 2026)

Ce guide a été conçu sur-mesure à partir de votre manuscrit de thèse et de vos présentations. Il structure vos deux jours à VivaTech pour maximiser les chances de succès de votre futur projet avec l'**Inria Startup Studio**, en ciblant les bons partenaires industriels (LiDAR, jumeaux numériques, CNDT, biotech, cyber) et en vous préparant aux conférences clés.

---

## 🎯 Objectifs de la Visite

1. **HGP-Clusterer 3D (Objectif N°1) :** Valider l'intérêt d'une API de clustering géométrique robuste (alternative à HDBSCAN) pour les acteurs du LiDAR 3D/4D et des jumeaux numériques (Dassault Systèmes, YellowScan, Wise Twin, CAD42).
2. **Applications Algorithmiques Secondaires (Objectif N°2) :** Valider l'attrait commercial de vos autres modèles théoriques :
    *   **Détection de Fissures (Signal/CNDT) :** Squelettisation par graphes de Frangi généralisés pour le contrôle d'infrastructures (SSNDT).
    *   **Assemblage d'Haplotypes (BioTech) :** Détection de communautés sur graphes signés (MCMC couplés) pour le séquençage génomique (Alithea Biotechnology).
    *   **Cybersécurité :** Application de vos modèles de graphes signés à la résolution 3-SAT (vérification/cryptanalyse) et à la détection d'intrusions réseau (Aikido Security, Cyberagentur).
3. **Parcours Inria Startup Studio (Objectif N°3) :** Suivre le programme de la **Learning Expedition (LEX)** de l'Inria et réseauter avec des investisseurs DeepTech (Bpifrance, Elaia, Partech, etc.) pour structurer la future startup.

---

## 🔒 Thème de Recherche Secondaire : Cybersécurité & Graphes

Vos travaux de thèse sur les graphes signés, la percolation et le clustering hiérarchique trouvent des applications directes dans le domaine de la cybersécurité. Voici comment vos modèles s'appliquent à ces données :

### A. Résolution du problème 3-SAT (Vérification formelle et Cryptanalyse)
*   **Données techniques :** Formules logiques CNF modélisant des propriétés de sécurité de logiciels (vérification de smart contracts, protocoles) ou des équations cryptographiques (collisions de hashs, clés privées).
*   **Modèles mathématiques :** Encodage de $3\text{-SAT}$ sous forme de graphes/hypergraphes signés. Introduction d'un nœud de référence $T$ (True) et construction de liens triangulaires (littéraux) et tétraédriques (avec $T$), où les signes encodent la logique de la clause. Résoudre la formule équivaut à minimiser l'énergie d'un modèle de spin (Spin Glass Ground State) via votre dynamique de Swendsen-Wang signée / triangulaire.
*   **Ce qu'on extrait :** Une affectation qui satisfait toutes les clauses, permettant de prouver la sécurité ou d'extraire un exploit (vulnérabilité).

### B. Détection d'Intrusions Réseau et Mouvements Latéraux
*   **Données techniques :** Graphes de flux réseaux (NetFlows) et graphes d'authentification (Active Directory) où les nœuds sont des utilisateurs/machines et les arêtes sont des connexions.
*   **Modèles mathématiques :** Stochastic Block Models (SBM) ou corrélation d'activités (attraction/répulsion). Utilisation de méthodes de percolation pour distinguer les bruits de fond du réseau (percolant) des attaques ciblées (isolées sous forme de petites communautés denses).
*   **Ce qu'on extrait :** Des sous-graphes d'anomalies représentant des botnets ou des mouvements latéraux.

### C. Classification de Malwares (Threat Intelligence)
*   **Données techniques :** Indicateurs de compromission (IOCs : signatures, appels API, clés de registre modifiées) partagés entre différents échantillons.
*   **Modèles mathématiques :** Correlation Clustering sur graphes signés (positif si IOCs partagés, négatif si comportements incompatibles). Votre algorithme MCMC probabiliste sur graphes signés permet de partitionner efficacement ces échantillons.
*   **Ce qu'on extrait :** Des familles de malwares (campagnes d'attaques coordonnées).

---

## 🗺️ Aperçu du Programme (Mercredi & Jeudi)

```mermaid
gantt
    title Programme VivaTech 2026
    dateFormat  HH:mm
    axisFormat %H:%M
    
    section Mercredi 17 Juin
    Arrivée & Accueil LEX Inria        :active, 14:00, 14:30
    Yann LeCun (VivaTech Theater)     : 14:30, 14:55
    Exploration & Sessions Stands (1) : 14:55, 17:30
    Débrief & Conférence Eklo Hotel   : 18:00, 19:30
    
    section Jeudi 18 Juin
    Café Stand Inria                  : 09:30, 09:45
    Conférence Quantum (Pasqal/IBM)   : 09:45, 10:45
    Conférence From Lab to Market     : 10:45, 11:30
    Conférence Free Models & Pricing  : 11:30, 12:00
    Déjeuner & Débrief Midi           : 12:00, 13:00
    Briefing & Planification CPPI     : 13:00, 14:00
    Conférence SaaS vs AI (Founders)  : 14:00, 14:45
    Conférence Cyber (Orange Cyber)   : 14:50, 15:35
    Pitchs Exposants Cibles (2)       : 14:45, 16:00
    Débrief Final LEX                 : 16:00, 16:30
```

---

## 🗓️ Mercredi 17 Juin 2026 : Validation de Marché & Prise de Contacts

> [!IMPORTANT]
> **Rendez-vous Inria LEX à 14h00** devant les grandes lettres **"VivaTech"** dans le hall principal pour le mot d'accueil des coordinateurs (Grégoire Maurice, Dylan Chomé, etc.).

### 🕒 Emploi du Temps
*   **14h00 - 14h30 :** Accueil officiel Inria Startup Studio et rencontre des autres doctorants.
*   **14h30 - 14h55 (Conférence Recommandée) :** *Beyond Language Models: Building AI that Understands the World* (**VivaTech Theater - Hall 7.3**).
    *   *Intervenant :* **Yann LeCun** (Meta, AMI Labs) en discussion avec Steven Levy (*Wired*).
    *   *Intérêt :* Entendre le pionnier du Deep Learning parler des représentations du monde et de la vision par ordinateur, hautement pertinent pour vos méthodes géométriques et vos modèles statistiques non paramétriques.
*   **14h55 - 17h30 (Temps Libre - Vos Cibles) :** Visite des exposants orientés **LiDAR/3D** et **Contrôle d'Infrastructures**.
    *   *Action :* Allez pitcher **Wise Twin**, **RESO3D** et cherchez le stand de **Dassault Systèmes** (demandez sa localisation exacte à l'accueil ou sur l'application mobile VivaTech).
*   **17h30 - 18h00 :** Déplacement vers l'hôtel Eklo.
*   **18h00 - 19h30 :** **Débriefing & Soirée Inria Startup Studio** (Hôtel Eklo Paris Porte de Versailles, *1 Rue du Moulin, 92170 Vanves*).
    *   *18h00 - 18h30 :* Débrief de l'après-midi.
    *   *18h30 - 19h00 :* Présentation du programme Inria Startup Studio.
    *   *19h00 - 19h30 :* Retours d'expérience de startups DeepTech, de VCs et de partenaires industriels. **(Moment idéal pour Alban pour discuter du montage financier/business de la future startup !)**

---

## 🗓️ Jeudi 18 Juin 2026 : Conférences DeepTech & Pitchs Exposants

> [!TIP]
> Ce deuxième jour est très rythmé, alternez entre les conférences du Founders Area / Purple Stage et vos visites de stands stratégiques.

### 🕒 Emploi du Temps
*   **09h30 - 09h45 :** Café réseau au **Stand Inria** (réparti sur les stands de Orange, La Poste, Caisse des Dépôts).
*   **09h45 - 10h45 (Conférence Recommandée) :** *Quantum Leap: When Will Quantum Computing Deliver Business Value?* (**Purple Stage - Hall 7.3**).
    *   *Intervenants :* Jerry Chow (IBM) & Loïc Henriet (Pasqal).
    *   *Intérêt :* Comprendre comment les grands algorithmes et les architectures de calcul intensif (comme Pasqal, spin-off académique français à succès) se structurent pour le marché B2B.
*   **10h10 - 10h30 (Optionnel - Réseau Inria) :** *Signature de l'accord Inria-DFKI* par **Bruno Sportisse** (CEO d'Inria) (**Startup Germany / German Park I**).
    *   *Intérêt :* Suivre la dynamique institutionnelle franco-allemande de l'Inria et réseauter avec la direction.
*   **10h45 - 11h30 (Conférence Majeure) :** *From Lab to Market* (**Founders Area - Hall 7.3**).
    *   *Intervenants :* Jacomo Corbo (PhysicsX) et Maximilien Levesque (Aqemia).
    *   *Intérêt :* **PhysicsX** fait du Deep Learning sur des maillages géométriques CAO et **Aqemia** est un spin-off d'Inria/ENS. C'est l'illustration parfaite de votre transition : vendre des algorithmes de pointe (complexes cellulaires, physiques) à l'industrie.
*   **11h30 - 12h00 :** *Selling When the Model is Free* (**Founders Area - Hall 7.3**).
    *   *Intérêt :* Indispensable pour votre modèle open-source / API hybride. Comment valoriser un algorithme mathématique lorsque le code de base est accessible ?
*   **12h00 - 13h00 :** Déjeuner libre (Food Court) et débriefing de la matinée.
*   **13h00 - 14h00 :** Session de connexion / Planification des visites avec le CPPI (Inria).
*   **14h00 - 14h45 (Conférence Recommandée) :** *Will AI Kill the SaaS Business Model by 2030?* (**Founders Area - Hall 7.3**).
    *   *Intérêt :* Réflexion cruciale sur le packaging de HGP-Clusterer (API SaaS vs. licence logicielle sur le edge pour les véhicules ou les serveurs locaux).
*   **14h50 - 15h35 (Conférence Cybersécurité) :** *AI vs. AI: The Race to Secure the Future* (**Purple Stage - Hall 7.3**). Table ronde avec **Hugues Foulon** (CEO de Orange Cyberdefense).
    *   *Intérêt :* Voir comment les modèles mathématiques prédictifs et les IAs autonomes luttent en temps réel contre les menaces.
*   **14h45 - 16h00 (Pitchs Cibles & Cyber) :** Visite des stands restants (**YellowScan**, **CAD42**, **SSNDT**, **Alithea**, et les exposants Cyber : **Aikido Security**, **Agentur für Innovation**).
*   **16h00 - 16h30 :** Débriefing final avec toutes les équipes Inria au Food Court.
*   **Après-midi (Optionnel - Réseau Inria) :** Discours de clôture de **Bruno Sportisse** pour l'atelier *"From Programming to Prompting: What Does Software Development Mean Today?"* (**Workshop Area B - Hall 7.3**).

---

## 🏢 Liste des Exposants Conseillés (Par ordre décroissant d'importance)

### 1. Dassault Systèmes
*   **Stand :** À localiser sur place via l'application mobile officielle VivaTech 2026 (ou aux bornes d'information).
*   **Objectif :** HGP-Clusterer 3D (Cible N°1).
*   **Informations clés :** Leader mondial des logiciels 3D et des jumeaux numériques (3DEXPERIENCE, CATIA).
*   **Détails & Synergies :** Leurs solutions industrielles ingèrent des nuages de points massifs issus de scans LiDAR pour reconstruire des scènes d'usines ou de villes. Ils intègrent des modèles physiques de substitution (surrogates) pour faire de la simulation mécanique en temps réel.
*   **Douleur client :** Le clustering de nuages de points denses et bruités est laborieux avec (H)DBSCAN.
*   **Votre valeur :** HGP-Clusterer 3D isole parfaitement les géométries complexes sans entraînement et gère les bruits de percolation (ponts de bruit) grâce aux Delaunay d'ordre $K$.

### 2. YellowScan
*   **Stand :** **Hall 7, Niveau 7.2**, à côté de "Mission French Tech".
*   **Objectif :** HGP-Clusterer 3D (Objectif N°1).
*   **Informations clés :** Leader mondial des systèmes LiDAR légers embarqués sur drones.
*   **Détails & Synergies :** Ils commercialisent la suite logicielle *CloudStation* (ground extraction, végétation, calibration d'intensité). Ils cherchent à automatiser la classification de lignes électriques, de câbles et de pylônes.
*   **Douleur client :** Extraire et segmenter des objets géométriquement complexes dans des données de vol très bruitées.
*   **Votre valeur :** HGP-Clusterer 3D permet d'injecter des *a priori* de volume faibles pour segmenter des instances 3D de manière robuste et sans entraînement.

### 3. Inria (Startup Studio)
*   **Stands :** Présent à travers les stands de ses partenaires : **Orange**, **La Poste**, **Caisse des Dépôts**, ainsi qu'au **German Park** et à l'**European Centre for AI Excellence**.
*   **Objectif :** Parcours Startup Studio (Objectif N°3).
*   **Informations clés :** L'institut national de recherche en sciences et technologies du numérique.
*   **Détails & Synergies :** Le programme Inria Startup Studio offre un accompagnement complet de 12 à 18 mois pour transformer une recherche académique en startup (salaires, mentoring, propriété intellectuelle).
*   **Votre intérêt :** Rencontrer l'équipe en personne pour cadrer votre candidature.

### 4. Bpifrance
*   **Stand :** **Stand 2F68** (Hall 7, Niveau 7.2, Business Plaza).
*   **Objectif :** Financement de la future startup (Objectif N°3).
*   **Informations clés :** Banque publique d'investissement française.
*   **Détails & Synergies :** Ils gèrent le *Plan Deeptech* national (Bourse French Tech, concours national *i-PhD*, prêts d'amorçage).
*   **Votre intérêt :** Alban doit comprendre les critères de ces subventions (association obligatoire recherche + business).

### 5. SSNDT (Smart Sensing and Non-Destructive Testing)
*   **Stand :** À localiser via l'application mobile officielle. *Note : Ils co-exposent généralement sur un pavillon thématique d'ingénierie, de contrôle industriel ou de recherche.*
*   **Objectif :** Détection de Fissures (Objectif N°2 - Signal/Image).
*   **Informations clés :** Acteur de l'auscultation d'infrastructures et du contrôle non destructif (CNDT).
*   **Détails & Synergies :** Ils développent des standards de sécurité diagnostique pour le génie civil (ex: béton armé) combinant capteurs intelligents et vision.
*   **Douleur client :** Détecter des micro-fissures peu visibles avec des images bruitées (optiques/thermiques) sans base d'apprentissage géante.
*   **Votre valeur :** Votre squelettisation par graphes de Frangi généralisés (Chapitre 12 de la thèse) fonctionne sans entraînement et fusionne efficacement les modalités visible/thermique.

### 6. Alithea Genomics (Alithea Biotechnology GmbH)
*   **Stand :** Pavillon swisstech / Suisse (à localiser via l'application mobile officielle). *Note : Alithea est une startup suisse basée à Lausanne.*
*   **Objectif :** Assemblage d'Haplotypes (Objectif N°2 - BioTech).
*   **Informations clés :** Spécialiste de la transcriptomique haut débit.
*   **Détails & Synergies :** Inventeurs de la technologie **BRB-seq** (Bulk RNA Barcoding and sequencing) qui marque individuellement les échantillons d'ARN dès la transcription inverse pour les séquencer en un seul tube (25x moins cher).
*   **Douleur client :** Reconstruire et assembler des fragments génomiques/ARN bruités ou dégradés à partir de ces lectures massives.
*   **Votre valeur :** Votre cadre bayésien de détection de communautés sur graphes signés (MCMC couplés, Chapitre 11.4) qui résout l'assemblage d'haplotypes sous fort bruit.

### 7. Agentur für Innovation in der Cybersicherheit GmbH (Cyberagentur)
*   **Stand :** À localiser dans l'espace Allemagne / German Park.
*   **Objectif :** Cybersécurité (Objectif N°2 - Cyber/SAT).
*   **Informations clés :** Agence publique allemande finançant la recherche de rupture en cybersécurité.
*   **Détails & Synergies :** Ils allouent des budgets de recherche à long terme (10-15 ans) pour la souveraineté technologique (quantique, IA, cryptographie post-quantique, sécurité spatiale).
*   **Votre intérêt :** Présenter vos approches de modélisation de SAT-solving via Swendsen-Wang sur graphes signés.

### 8. Aikido Security
*   **Stand :** À localiser sur place via l'application mobile.
*   **Objectif :** Cybersécurité (Objectif N°2 - Vérification logicielle).
*   **Informations clés :** Solution de sécurité applicative unifiée (SAST/DAST/Cloud).
*   **Détails & Synergies :** Aikido intègre de nombreux scanners de vulnérabilités et déploie un moteur de tri (*de-noising*) pour éliminer les faux positifs en fonction du contexte de production.
*   **Votre intérêt :** Discuter des moteurs de détection de vulnérabilités basés sur des solveurs de contraintes logiques (SAT Solving).

### 9. Wise Twin
*   **Stand :** **Stand 3H14** (Hall 7.3, pavillon IMT - Institut Mines-Télécom). *Note : Ils y exposent sur le thème "transition industrielle+" le jeudi 18 juin.*
*   **Objectif :** HGP-Clusterer 3D (Jumeaux Numériques).
*   **Informations clés :** Startup de jumeaux numériques pour le domaine industriel et portuaire.
*   **Détails & Synergies :** Ils capturent des nuages de points 3D de sites industriels complets pour en faire des modèles géométriques.
*   **Douleur client :** Segmenter et classifier automatiquement chaque objet physique (grues, containers, tuyauteries) à partir des points bruts.
*   **Votre valeur :** HGP-Clusterer 3D permet d'automatiser cette segmentation géométrique sans données d'entraînement.

### 10. RESO3D
*   **Stand :** **Stand 3C14** (Hall 7, pavillon Région Sud). *Note : RESO3D fait partie de la délégation officielle de la Région Sud.*
*   **Objectif :** LiDAR 3D.
*   **Informations clés :** Spécialiste de la cartographie 3D de réseaux souterrains.
*   **Détails & Synergies :** Ils modélisent les réseaux enterrés (canalisations, câblages) par photogrammétrie et scan 3D.
*   **Douleur client :** Extraire des tuyaux et câbles continus dans des nuages de points fragmentés et bruités par les débris des excavations.
*   **Votre valeur :** Votre approche d'extraction de réseaux par graphes de centralité et de percolation (Chapitre 12 de la thèse) s'applique directement à l'extraction de structures tubulaires.

### 11. CAD42
*   **Stand :** À localiser via l'application mobile officielle (co-exposant possible sur un pavillon BTP/construction ou innovation industrielle).
*   **Objectif :** LiDAR / Suivi 3D.
*   **Informations clés :** Suivi 3D en temps réel et sécurité sur chantiers.
*   **Détails & Synergies :** Ils développent des systèmes anticollision embarqués sur grues s'appuyant sur des capteurs spatiaux et du tracking temps réel.
*   **Votre intérêt :** Discuter de vos modèles de suivi temporel robuste d'instances 3D/4D (tracking d'instances sur nuages de points).

---

## 🎙️ Liste des Speakers & Conférences (Par ordre décroissant d'importance)

### 1. Jacomo Corbo (PhysicsX) & Maximilien Levesque (Aqemia)
*   **Conférence :** *From Lab to Market with PhysicsX, Aqemia, Qobly and Connected Circles*
*   **Date & Heure :** **Jeudi 18 Juin, 10h45 – 11h30** | **Lieu :** **Founders Area (Hall 7.3)**
*   **Détails & Synergies :**
    *   **Jacomo Corbo (PhysicsX) :** Ex-ingénieur en chef stratégie F1 (Renault Team). *PhysicsX* utilise le Deep Learning géométrique (sur meshes/point clouds) pour accélérer par $10\thinspace 000$ les simulations physiques de CAO (CFD, FEA).
    *   **Maximilien Levesque (Aqemia) :** Ex-CNRS et ENS. *Aqemia* utilise des algorithmes de physique statistique et quantique (équation d'Ornstein-Zernike) pour générer ses propres données d'affinités chimiques et concevoir des médicaments sans données d'entraînement historiques.
    *   **Pourquoi :** Le modèle absolu à suivre : comment des algorithmes physiques et géométriques complexes se traduisent en API commerciale B2B.

### 2. Yann LeCun (Meta, AMI Labs)
*   **Conférence :** *Beyond Language Models: Building AI that Understands the World* (avec Steven Levy, *Wired*)
*   **Date & Heure :** **Mercredi 17 Juin, 14h30 – 14h55 CET** | **Lieu :** **VivaTech Theater (Hall 7.3)**
*   **Détails & Synergies :** Lauréat du prix Turing et directeur de l'IA chez Meta. Ses recherches sur les *World Models* et la vision auto-supervisée visent à donner aux machines une compréhension spatio-temporelle intuitive du monde.
*   **Pourquoi :** Son point de vue sur la vision par ordinateur est très proche de vos approches non-paramétriques et de percolation géométrique.

### 3. Bruno Sportisse (CEO d'Inria)
*   **Événement N°1 :** *Signing of the Franco-German Center on AI / DFKI-Inria Agreement*
    *   **Date & Heure :** **Jeudi 18 Juin, 10h10 – 10h30** | **Lieu :** **Startup Germany / German Park I**
*   **Événement N°2 :** *Closing remarks: From Programming to Prompting*
    *   **Date & Heure :** **Jeudi 18 Juin, Après-midi** | **Lieu :** **Workshop Area B (Hall 7.3)**
*   **Détails & Synergies :** PDG de l'Inria et mathématicien appliqué. Il pilote la stratégie nationale de valorisation Deeptech d'Inria (Inria Startup Studio).
*   **Pourquoi :** Indispensable pour votre frère et vous pour comprendre les mécanismes institutionnels et valider votre projet de startup.

### 4. Hugues Foulon (CEO d'Orange Cyberdefense)
*   **Conférence :** *AI vs. AI: The Race to Secure the Future*
*   **Date & Heure :** **Jeudi 18 Juin, 14h50 – 15h35** | **Lieu :** **Purple Stage (Hall 7.3)**
*   **Détails & Synergies :** Dirige le premier prestataire européen de sécurité managée. Ses équipes surveillent les réseaux à grande échelle et intègrent l'IA prédictive et la détection d'intrusions.
*   **Pourquoi :** Roundtable clé pour comprendre les besoins actuels en termes de modèles de détection et de graphes de flux réseau.

### 5. Jerry Chow (IBM Quantum) & Loïc Henriet (Pasqal)
*   **Conférence :** *Quantum leap: when will quantum computing deliver business value?*
*   **Date & Heure :** **Jeudi 18 Juin, 09h45 – 10h45** | **Lieu :** **Purple Stage (Hall 7.3)**
*   **Détails & Synergies :** Jerry Chow gère les architectures quantiques IBM. Loïc Henriet pilote Pasqal, spin-off académique français qui conçoit des processeurs quantiques à atomes neutres. Leurs processeurs résolvent des problèmes complexes d'optimisation de graphes (Maximum Independent Set).
*   **Pourquoi :** Comprendre comment commercialiser des calculateurs et algorithmes de rupture auprès de grands groupes.

---

## 🗣️ Fiches de Pitch Rapide (2 minutes)

### Pitch A : HGP-Clusterer (Pour Dassault, YellowScan, Wise Twin)
> *"Bonjour, je suis Louis Hauseux, chercheur à l'Inria et futur fondateur de startup, et voici mon frère et associé business, Alban Hauseux. Dans le traitement de nuages de points LiDAR 3D, tout le monde utilise (H)DBSCAN pour la segmentation d'instances. Mais (H)DBSCAN échoue dès qu'il y a du bruit ou des densités variables : il crée des ponts et fusionne des objets distincts.
> Mes travaux de thèse ont résolu ce problème en généralisant le Single-Linkage avec la géométrie des complexes de Čech et des Delaunay d'ordre K. Notre algorithme, **HGP-Clusterer**, est mathématiquement robuste au bruit et permet d'injecter des contraintes physiques (comme le volume estimé des objets) pour segmenter des scènes LiDAR urbaines ou industrielles sans aucun entraînement profond. Nous voulons proposer cela sous forme d'une API plug-and-play."*

### Pitch B : Détection de Fissures (Pour SSNDT)
> *"Bonjour, nous développons une technologie d'extraction de structures filaires pour le contrôle non destructif. Contrairement aux approches Deep Learning qui nécessitent des milliers d'images annotées et peinent sur les fissures très fines ou bruitées, notre approche repose sur des modèles géométriques explicites. En étendant le filtre de Frangi sous forme de graphe spatial et en utilisant des métriques de centralité et de percolation, nous extrayons des squelettes de fissures parfaits, même sur des acquisitions multimodales (visible + thermique). Le code est léger, explicite et fonctionne sans phase d'apprentissage."*

### Pitch C : Cybersécurité / Modèles de Graphes (Pour Cyberagentur, Aikido)
> *"Bonjour, je suis Louis Hauseux, chercheur à l'Inria, et voici Alban, mon associé business. Nos travaux portent sur l'application de la théorie des graphes et des modèles de spin statistiques à la structuration de données bruitées. En cybersécurité, nous appliquons nos modèles de graphes signés (MCMC couplés et percolation) à la résolution ultra-rapide de formules 3-SAT pour la vérification de code et la cryptanalyse, mais aussi à la détection probabiliste de botnets et de mouvements latéraux dans les graphes de flux réseau. Nous cherchons à valider des cas d'usage industriels pour ces modèles mathématiques."*

---

## 📂 Documents de Référence dans le Workspace

Pour retrouver les détails techniques durant vos trajets ou vos temps de pause :
*   Le manuscrit complet : [Manuscrit de thèse](file:///workspaces/VivaTech2026/Manuscrit_de_thèse_LouisHauseux_2026-06-15.pdf)
    *   *Détails HGP-Clusterer :* Chapitre 6 (p. 51) et Chapitre 9 (p. 93).
    *   *Détails Assemblage Haplotypes :* Chapitre 11, Section 11.4 (p. 141).
    *   *Détails Détection de Fissures :* Chapitre 12 (p. 145).
*   Les slides de présentation générale HGP : [Présentation HGP (B. Levy)](file:///workspaces/VivaTech2026/PresentationBrunoLevy_2026-06.pdf)
*   Les slides Graphes Signés & Haplotypes : [Présentation MathNet (Signed Graphs)](file:///workspaces/VivaTech2026/PresentationMathNet_2026-06-15_LouisHauseux_ABayesianFrameworkForCommunityDetectionOnSignedGraphs.pdf)
*   Les infos logistiques de la LEX : [Présentation LEX Inria Startup Studio](file:///workspaces/VivaTech2026/Présentation LEX VT26.pptx)
