---
format:
  html:
    theme: cosmo
    keep-md: true
    keep-tex: true
    tbl-colwidths: auto
  pdf:
    include-in-header:
      text: |
        \addtokomafont{disposition}{\rmfamily}
        \usepackage{placeins}
        \usepackage{fancyhdr}
        \usepackage{setspace}
        \usepackage{chngcntr}
        \usepackage{microtype}
        \usepackage{tabularx}
        \usepackage{tabularray}
        \usepackage{longtable}
        \usepackage{newcomputermodern}
        \onehalfspacing
        \counterwithin{figure}{section}
        \counterwithin{table}{section}
    include-before-body:
      - columns.tex
editor: visual
output: 
  pdf_document:
    citation_package: natbib
    keep_tex: true
    fig_caption: true
    number_sections: true
    latex_engine: pdflatex
    pandoc_args: [
       "--filter", "pandoc-citeproc"
     ]
lang: fr
filters: 
  - multibib.lua
  - parse-latex
    # template: svm-latex-cv.tex
title: "Notice individuelle"
author:
- name: Julien Le Roux
affiliation: Université Paris-Est-Créteil
keywords: "pandoc, r markdown, knitr"
date: "02 02 2026"
geometry: margin=1in
fontsize: 11pt
# spacing: double
csl: american-chemical-society-b.csl
link-citations: true
---

---
bibliography:
  papersint: papers-int.bib
  papersnat: papers-nat.bib 
  comintorale: com-int-orale.bib 
  comintaff: com-int-aff.bib 
  comnatorale: com-nat-orale.bib 
  comnataff: com-nat-aff.bib 
  chap: chapters.bib 
  data: datasets.bib 
  software: software.bib
  video: videos.bib
---

---
nocite: '@*'
---







\pagenumbering{gobble}

\newpage
\pagestyle{fancy}
\fancyhead[LE,RO]{}
\fancyhead[LO,RE]{}
\renewcommand{\headrulewidth}{0.4pt}
\renewcommand{\footrulewidth}{0pt}

\pagenumbering{roman}

\newpage
\fancyhead[CO,CE]{Table des matières}
\setcounter{tocdepth}{2}
\tableofcontents
\newpage
\pagenumbering{arabic}
\newpage
\fancyhead[CO,CE]{Curriculum Vitae}

# 1. Curriculum Vitae










```{=tex}
\begin{centering}

\vspace{1 cm}

\huge
Julien Le Roux

\vspace{1 cm}

\Large
Ingénieur en Traitement des Eaux et des Nuisances\\ 

Docteur en Sciences de l'Eau \\

Maître de conférences (5\textsuperscript{e} échelon), 35\textsuperscript{e} section CNU

\vspace{1 cm}

\large
Né le 29 novembre 1985 à Nantes\\ 
\vspace{5mm}
\textbf{Coordonnées professionnelles}\\
\normalsize 
Université Paris-Est Créteil - Maison des Sciences de l'Environnement\\
5 rue Pasteur Vallery-Radot\\
94000 Créteil, France\\
\vspace{5mm}
01 82 39 20 80\\
julien.le-roux@u-pec.fr

\end{centering}

\DefTblrTemplate{contfoot-text}{default}{}
\DefTblrTemplate{conthead-text}{default}{}
\DefTblrTemplate{caption}{default}{}
\DefTblrTemplate{conthead}{default}{}
\DefTblrTemplate{capcont}{default}{}

\begin{longtblr}{r | p{13cm}}

2008 & Diplôme d’Ingénieur de l’\textbf{École Supérieure d’Ingénieurs de Poitiers (ESIP)} – Spécialité Eau et Environnement\\
& Diplôme de Master 2 Recherche Chimie et Applications, spécialité Chimie et Microbiologie des Eaux | \small\emph{mention bien} - \textbf{Université de Poitiers}\\
& Sujet de Master : « \emph{Etude du pouvoir colmatant de quelques eaux souterraines} » | \small Direction : Jean-Philippe \textsc{Croué} (ENSI Poitiers) \& Bénédicte \textsc{Welté} (Eau de Paris)\\
&\\


2008-2011 & Doctorat de Chimie spécialité Chimie et Microbiologie de l’Eau – \textbf{École Nationale Supérieure d’Ingénieurs de Poitiers (ENSIP), Université de Poitiers}\\
& Allocataire de recherche et moniteur\\
& Thèse : « \emph{Mécanisme de formation des nitrosamines et sous-produits halogénés lors de la chloramination de contaminants organiques azotés émergents} » | \small Direction : Jean-Philippe \textsc{Croué} \& Hervé \textsc{Gallard}\\
&\\
&\\


2011-2012 & Attaché Temporaire d’Enseignement et de Recherche (ATER) à l’\textbf{ENSI Poitiers}, France\\
& \small{Enseignements en Chimie des eaux et traitement des eaux}\\
&\\


2012-2014 & Chercheur Post-Doctoral au \textsc{Water Desalination and Reuse Center} (WDRC), \textbf{Université KAUST}, Arabie Saoudite\\
& \small{Thématiques de recherche : 
\newline $\rightarrow$ Identification de sous-produits de désinfection dans des usines de dessalement (Mer Rouge)
\newline $\rightarrow$ Projet avec l’Université d’Illinois à Urbana-Champaign : « Nitrogenous DBPs in Reclaimed Wastewater Effluents: Chemistry, Toxicity and Control Strategies ».
\newline $\rightarrow$ Identification de produits d'oxydation avancée par LC-ORBITRAP et LC-MS\textsuperscript{n}
\newline $\rightarrow$ Identification de sous-produits de désinfection formés à partir d’effluents d’eaux usées
\newline $\rightarrow$ Utilisation avancée de techniques analytiques : GC-ICP-MS, LC-QTOF, LC-ORBITRAP}\\
&\\


Depuis 2015 & Maitre de conférences au \textsc{Laboratoire Eau Environnement et Systèmes Urbains (LEESU)}, \textbf{Université Paris-Est Créteil}\\
& \small{Enseignements en chimie à l’UPEC (Faculté des Sciences et Technologie), niveaux L1 à M2\\
Thématiques de recherche : 
\newline $\rightarrow$ Mécanismes de transfert et de transformation de polluants organiques dans les eaux urbaines : caractérisation, compréhension, quantification
\newline $\rightarrow$ Traitement avancé de micropolluants organiques dans les effluents d’eaux usées
\newline $\rightarrow$ Développement analytique en spectrométrie de masse haute résolution}\\
&\\

Depuis 2017 & Co-responsable du master en apprentissage \textsc{Analyse et Assurance Qualité} de la Faculté des Sciences et Technologie de l'\textbf{Université Paris-Est Créteil}. Organisation du passage de la formation sur 2 années à partir de 2020.\\
&\\

2022 & Titulaire de la prime individuelle RIPEC.
&\\

\end{longtblr}
```





\FloatBarrier
\newpage
\fancyhead[CO,CE]{Activités de recherche}

# 2. Activités de recherche

## 2.1 Projets de recherche

### Porteur de projets

\twocolsection{}{
2017 & Appel à projet de la Faculté de Sciences et Technologie de l'UPEC - soutien à la recherche des Maîtres de Conférences nouvellement nommés. « \emph{Caractérisation de micropolluants organiques dans les procédés de traitement des eaux} » 6,1 k€.\\

2016-2019 & projet \emph{Carboplus} (OPUR 4 - financement SIAAP, collectivités territoriales, Agence de l'Eau) : « \emph{Abattements des polluants prioritaires et émergents par charbon actif} ». Co-direction de thèse de Ronan \textsc{Guillossou}. 150 k€.\\

2016-2021 & ANR JCJC \emph{WaterOmics} : « \emph{Traquer les micropolluants organiques dans les eaux urbaines par spectrométrie de masse haute résolution : approches omiques, empreintes et indices} ». Co-direction de thèse de Nina \textsc{Huynh} + 2 stages de M2. 272 k€.\\

2018-2019 & Appel à post-doc UPEC / programme PRESTIGE (Campus France) : « \emph{Caractérisation de micropolluants organiques dans les procédés d'oxydation avancée (UV/H\textsubscript{2}O\textsubscript{2} et UV/PDS) des eaux usées} ». Co-direction de post-doctorat (Maolida \textsc{Nihemaiti}) 12 mois de salaire + 4 k€ de fonctionnement.\\

2019-2022 & OPUR 5 (financement SIAAP, collectivités territoriales, Agence de l'Eau) : Action R2.5 : « \emph{Elimination de micropolluants en traitement tertiaire des eaux usées par différents procédés d'oxydation} ». Co-direction de thèse (Christelle \textsc{Nabintu Kajoka}). 150 k€.\\

2019-2022 & OPUR 5 : Action R2.6 : « \emph{Nouvelles méthodes de caractérisation des micropolluants : analyses par screening non-ciblé et écotoxicologie} ». 80 k€.\\

2020 & Prestation analytique « \emph{analyse d'échantillons de Seine et de sols suite à l'incendie de l'usine Lubrizol à Rouen} ». 2 mois de salaire de post-doc (Maolida \textsc{Nihemaiti}).\\

2021-2023 & Partenaire de l'ANR RA-SIOMRI 2021 (Recherche-Action - Solutions innovantes et opérationnelles dans la maitrise des risques industriels en milieu urbain et dense) \emph{ENVAHY} : « \emph{Imprégnation de l'ENVironnement suite à un Accident industriel en milieu urbain dense : recherche de marqueurs et de leur transfert dans l'Hydrosystème} », portée par M. \textsc{Fournier} (Université de Rouen Normandie). Financement d'un stage de M2 + fonctionnement. 18,3 k€.\\

2021-2024 & Programme MeSeine Innovation (Observer et comprendre la Seine francilienne), Phase 1 : Action 2.2.2 : « \emph{Caractérisation de la contamination des eaux de surface par le couplage d’analyses non-ciblées en spectrométrie de masse avec des analyses d’écotoxicologie} ». Porteur de l'action. Co-direction de thèse (Julien \textsc{Sade}).\\

2022-2025 & Projet Européen HORIZON-WIDERA-2021-ACCESS-02-01 - Twinning Western Balkans Special. \emph{SmartWaterTwin} : « \emph{Twinning for smart water - thinking and rethinking wastewater management in circular economy frame} ». Porté par l'Université de Novi Sad (Serbie), partenaires ICRA (Espagne) et UPEC (France) : porteur pour la France. 247 k€.\\

2024-2027 & Projet ADEME APR GRAINE 2024 - Production, valorisation des biomasses et préservation des écosystèmes : la bioéconomie face aux enjeux climatiques et environnementaux. \emph{FreezePee} : « \emph{Evaluation d'un procédé novateur de cryoconcentration : élaboration, analyse et démonstration d'un nouvel urino-fertilisant} ». Porteur du projet (UPEC), partenaires : Ecole Nationale des Ponts et Chaussées, INRAE, Terre et Cité, Chambre d'Agriculture de région Ile-de-France. 300 k€.\\

2024-2027 & Projet \emph{ChemBiodiv} : « \emph{Relier la pression chimique à ses effets sur la biodiversité dans les eaux urbaines} ». Financements EUR Live (financement de thèse de Ravo Ravaorafindrasoa), Région Ile-de-France (financement de thèse de Malek Baroudi) et SIAAP (programme MeSeine Innovation, Action 2.2.3). Porté avec Adèle Bressy et My Dung Jusselme. 270 k€.\\

2025-2027 & Projet ECOS-Sud. \emph{AQUASOL} : « \emph{Franco-Chilean Innovation for Solar Wastewater Treatment with Micropollutants, Microorganisms and ARG Elimination Focus} », Collaboration avec la Pontificia Universidad Católica de Chile (Chili) (Pr. Ricardo Salazar González), financement de séjours de chercheurs confirmés et doctorants.\\
}

### Implications dans d'autres projets

\twocolsection{}{
2016 & PICRI \emph{ReFUJ} : « \emph{Reconversion d'une Friche Urbaine en Jardin} ». Porté par M. \textsc{Bagard}. Co-encadrement d'un stagiaire de M2 avec M. \textsc{Seidl}.\\

2017 & Appel à projet collaboratif de l’OSU-EFLUVE (UPEC) : \emph{Screenatm’eau} : « \emph{Développement d’une méthode non ciblée pour l’analyse de micropolluants par couplage chromatographie liquide et spectrométrie de masse haute résolution à l’interface eau/atmosphère} ». Porté par A. \textsc{Bressy}. 18 k€.\\

2014-2019 & Appel à projet AESN/OFB : \emph{Roulépur} : « \emph{Caractérisation expérimentale de la rétention et du devenir de micropolluants dans le sol d’un ouvrage de gestion des eaux de ruissellement de voirie} » Implication dans l’encadrement d’une stagiaire de M2 (6 mois). Porté par M.C. \textsc{Gromaire}.\\

2019-2022 & OPUR 5 : Thème O2 « \emph{Observatoire des micropolluants dans les eaux urbaines} ». Porté par R. \textsc{Moilleron}.\\

2021-2025 & Participation à l’ANR JCJC (AAPG 2021) \emph{Biocid$@$Home} : « \emph{Biocides at home: emissions, potential exposure and reduction solutions} », portée par A. \textsc{Bressy}. 352 k€.\\

2021-2025 & Participation à l’ANR PRC (AAPG 2021) \emph{EGOUT} : « \emph{Extended Geochemical Observation of Urban Trajectories} », portée par J. \textsc{Jacob} (LSCE). 685 k€.\\

2023-2024 & Appel à projet "Amorçage" de la ComUE Paris-Est Sup : \emph{Electr'Eau} : « \emph{Traitement tertiaire des eaux usées municipales par électro-oxydation : élimination des micropolluants et estimation du risque en cas de réutilisation} », porté par C. \textsc{Trellu} (LGE - Université Gustave Eiffel). 35 k€.\\

2023-2024 & Participation au projet C-BASC 2022 (Université Paris-Saclay) : \emph{MedUrinAgri} : « \emph{Evaluation ciblée et non-ciblée de résidus de médicaments dans des urines traitées ou stockées et dans les sols les recevant} », porté par M. \textsc{Deschamps} (UMR ECOSYS) et C. \textsc{Aubry} (UMR SADAPT). 30 k€.\\

2024-2027 & Participation au projet CASDAR FranceAgriMer : \emph{Pluvaluh} : « \emph{Promouvoir L'Usage et la Valorisation en Agriculture de L'Urine Humaine} », porté par la Chambre d’Agriculture de Région Ile-de-France. 588 k€.\\

}

## 2.2 Encadrements

### Post-doctorants

\twocolsection{}{
2018-2019 & Maolida \textsc{Nihemaiti}, \textbf{post-doctorante de l'Université Paris-Est Créteil}, appel à projet UPEC et programme PRESTIGE (Campus France/Union
Européenne)\\
  & \small\emph{Caractérisation de micropolluants organiques dans les procédés d’oxydation (acide performique) des eaux usées}\\
  
2024-2027 & Corentin \textsc{Eschenbrenner}, \textbf{post-doctorant de l'Université Paris-Est Créteil}, appel à projet de recherche GRAINE de l'ADEME\\
  & \small\emph{Evaluation d'un procédé novateur de cryoconcentration : élaboration, analyse et démonstration d'un nouvel urino-fertilisant}\\
  
2026-2028 & Sylvain \textsc{Faixo}, \textbf{post-doctorant de l'Université Paris-Est Créteil}, projet de recherche avec SUEZ\\
  & \small\emph{Traitement des micropolluants dans les eaux usées : étude de l'efficacité de procédés et de caractérisation des mécanismes d'élimination par spectrométrie de masse haute résolution}\\
}


### Doctorants

\twocolsection{}{
  2016-2019 & Ronan \textsc{Guillossou}, \textbf{doctorant de l'Université Paris-Est}, Ecole des Ponts ParisTech, programme OPUR\\
  & \small\emph{Elimination des micropolluants organiques dans les eaux résiduaires urbaines par adsorption sur charbon actif : compréhension des processus et implications opérationnelles} | \small Encadrement à 50~\%, co-direction : J. \textsc{Gasperi}\\
  &\\
  %------------------------------------------------

  2018-2022 & Nina \textsc{Huynh}, \textbf{doctorante de l'Université Paris-Est Créteil}, programmes de recherche WaterOmics \& OPUR\\
  & \small\emph{Caractérisation des eaux résiduaires urbaines par spectrométrie de masse haute résolution : influence de la stratégie analytique, limitations et perspectives} | \small Encadrement à 75~\%, co-direction : R. \textsc{Moilleron}\\
  &\\
  %------------------------------------------------

  2020-2023 & Christelle \textsc{Nabintu Kajoka}, \textbf{doctorante de l'Ecole des Ponts ParisTech}, programme OPUR\\
  & \small\emph{Utilisation de l’acide performique en traitement des eaux résiduaires urbaines : réactivité avec les micropolluants organiques et stratégies d’intégration au sein de procédés d’oxydation avancée} | \small Encadrement à 40~\%, co-direction : G. \textsc{Chebbo}, J. \textsc{Gasperi}, S. \textsc{Brosillon}\\
  & \small Lauréate 2024 d'un prix de thèse de la ComUE Paris-Est Sup (prix spécial "Territoire")\\
  &\\
  %------------------------------------------------

  2021-2024 & Julien \textsc{Sade}, \textbf{doctorant de l'Université Paris-Est Créteil}, programme MeSeine Innovation\\
  & \small\emph{Caractérisation de la contamination des eaux de surface par le couplage d’analyses non-ciblées en spectrométrie de masse avec des analyses d’écotoxicologie} | \small Encadrement à 50~\%, co-direction : R. \textsc{Moilleron}, S. \textsc{Mottelet}\\
  &\\
  %------------------------------------------------
  
  2024-2027 & Ravo \textsc{Ravaozafindrasoa}, \textbf{doctorant de l'Université Paris-Est Créteil}, Ecole de Recherche Universitaire EUR Live (Life Trajectories \& Health Vulnerability)\\
  & \small\emph{Peut-on prévoir la vulnérabilité sanitaire des ressources en eau en couplant la pression chimique à l'ADN environnemental ?} | \small Encadrant principal (40~\%) - co-direction : A. \textsc{Bressy}, M.D.  \textsc{Jusselme}\\
  &\\
  %------------------------------------------------
  
  2024-2027 & Malek \textsc{Baroudi}, \textbf{doctorante de l'Ecole Nationale des Ponts et Chaussées}, Financement Région Ile-de-France\\ 
  & \small\emph{Antibiorésistance et micropolluants dans les écoystèmes aquatiques : intégration des données issues de la métagénomique et de l’analyse HRMS non-ciblée, de la station d’épuration au milieu récepteur} | \small Encadrement à 30~\% - co-direction : A. \textsc{Bressy}, M.D. \textsc{Jusselme}\\
  &\\
  %------------------------------------------------
  
  2024-2027 & Birsu \textsc{Guzel}, \textbf{doctorante de l'Université Paris-Est Créteil}, programme de recherche Mocopée\\ 
  & \small\emph{Dynamique des pathogènes dans le cycle de l'eau : de l'entrée à la sortie des stations d'épuration (STEP) : analyse de l'efficacité des traitements avancés} | \small Encadrement à 15~\% - co-direction : R. \textsc{Moilleron}, M.D. \textsc{Jusselme}\\
  &\\
  %------------------------------------------------

  2025-2028 & Rémi \textsc{Belleau}, \textbf{doctorant de l'Université Paris-Est Créteil}, programme de recherche OPUR et IUT Sénart-Fontainebleau (UPEC)\\ 
  & \small\emph{Caractérisation chimique et écotoxicologique de la contamination en micropolluants organiques et microplastiques dans les matières fertilisantes d'origine résiduaire en contexte urbain} | \small Encadrement à 50~\% - co-direction : R. \textsc{Moilleron}, T. \textsc{Tambosco}\\
}

### Stagiaires

\twocolsection{}{ 
2015 & \textbf{Shintuya \textsc{Sivayanama}}, Licence 3 Chimie-Biologie Université Paris-Est Créteil, 2 mois. \small\emph{Etude de la conservation des échantillons environnementaux - Suivi des paramètres globaux de qualité des eaux}\\

2016 & \textbf{Amina \textsc{Azzaoui}}, Licence 3 Chimie Université Paris-Est Créteil \& \textbf{Clarisse \textsc{Gayen}}, licence 3 SVT parcours Chimie-Biologie Université Paris-Est Créteil, 2 mois. \small\emph{Evaluation de l’impact de rejets urbains et de polluants organiques sur la qualité des eaux de surface par une approche métabolomique}\\

& \textbf{Rémi \textsc{Mazerolles}}, Master 2 TVRN, option TQE, Université de Picardie Jules Vernes, ESCOM, 6 mois. \small\emph{Impact des friches industrielles sur la qualité des nappes phréatiques - le cas du site de la Pierre-Fitte à Villeneuve-le-Roi} | \small Co-encadrement : M. \textsc{Seidl}\\

& \textbf{Thi Kim Phung \textsc{Nguyen}}, Master 2 Systèmes Aquatiques et Gestion de l'Eau, 6 mois. \small\emph{Caractérisation expérimentale de la rétention et du devenir de micropolluants dans le sol d’un ouvrage de gestion des eaux de ruissellement de voirie} | \small Co-encadrement : M.C. \textsc{Gromaire}\\

2018 & \textbf{Hadley \textsc{Habeck}}, Master 1 Université Paris-Est Créteil/Northern Arizona University, 4 mois. \small\emph{Développement de méthodes pour l’analyse de contaminants dans les eaux urbaines : substituts aux parabènes par LC/MSMS, sous-produits d’oxydation par GC/MSMS}\\

& \textbf{Jérémy \textsc{Guyot}}, Master 2 Systèmes Aquatiques et Gestion de l'Eau, 6 mois. \small\emph{Développement de méthodes pour l’analyse de contaminants organiques dans les eaux urbaines par spectrométrie de masse haute résolution}\\

2019 & \textbf{Hans \textsc{Tshimika}}, Licence 3 Chimie Université Paris-Est Créteil, 2 mois. \small\emph{Caractérisation des eaux urbaines par spectrométrie de masse : extraction et fractionnement de matière organique et de micropolluants} | Encadrement avec Nina Huynh\\

2020 & \textbf{Emma \textsc{Seon}}, Master 1 Toxicologie Université de Paris, 2 mois. \small\emph{Caractérisation des micropolluants organiques dans les eaux résiduaires par analyse EDA (effect directed analysis)} | Encadrement avec Nina Huynh\\

& \textbf{Fatoumata \textsc{Signate}}, BTS Métiers de la Chimie 2\textsuperscript{e} année ENCPB, 2 mois. \small\emph{Caractérisation de sous-produits d’oxydation et évaluation de leur toxicité dans les eaux usées} | Encadrement avec Nina Huynh\\

2021 & \textbf{Alicia \textsc{Cotard}}, Master 2 Quatro, Ecole Nationale Supérieure d'Ingénieurs de Limoges, 6 mois. \small\emph{Etude du comportement des micropolluants organiques au sein de bioréacteurs à membranes en traitement des eaux usées urbaines} | Encadrement avec Romain Mailler et Melissa Lopez Viveros, SIAAP\\

& \textbf{Lamyae \textsc{El Mrabet}}, Master 2 Chimie Université de Limoges, 6 mois. \small\emph{Caractérisation par spectrométrie de masse haute résolution de produits de dégradation lors de l’oxydation de micropolluants organiques} | Encadrement avec Nina Huynh\\

& \textbf{Maysar \textsc{Bouslah}}, BTS Métiers de la Chimie 2\textsuperscript{e} année ENCPB, 2 mois. \small\emph{Oxydation de Micropolluants organiques par l’acide performique} | Encadrement avec Christelle Nabintu Kajoka\\

2022 & \textbf{Lamyae \textsc{El Mrabet}}, Master 2 Systèmes Aquatiques et Gestion de l'Eau, 6 mois. \small\emph{Développements méthodologiques et identification de marqueurs d’un incendie industriel dans les phases aqueuses, les sédiments et les sols (projet ENVAHY)}\\

& \textbf{Chaimae \textsc{Messah}}, Master 1 Pro CAC Université de Bourgogne, 6 mois. \small\emph{Mise au point de méthodes analytiques pour la quantification de micropolluants émergents dans les boues d’épuration} | Co-encadrement avec Melissa Lopez Viveros, SIAAP\\

& \textbf{Melissia \textsc{Ben Iken}}, Licence 3 Chimie Université Paris-Est Créteil, 4 mois. \small\emph{Oxydation des micropolluants organiques par l'acide performique : cinétique, sous produits et mécanismes d'oxydation} | Encadrement avec Christelle Nabintu Kajoka\\

& \textbf{Ilyess \textsc{Taïbi}}, BTS Métiers de la Chimie 2\textsuperscript{e} année ENCPB, 2 mois. \small\emph{Oxydation de Micropolluants organiques par l’acide performique} | Encadrement avec Christelle Nabintu Kajoka\\

2023 & \textbf{Leila \textsc{Ibrahim}}, Licence 3 Chimie Université Paris-Est Créteil, 4 mois. \small\emph{Oxydation des micropolluants organiques par l'acide performique : cinétique, sous produits et mécanismes d'oxydation} | Encadrement avec Christelle Nabintu Kajoka\\

& \textbf{Antoine \textsc{Le Clair}}, Master 2 Chimie Sorbonne Université, 6 mois. \small\emph{Optimisation de méthodes d'analyse ciblée et non-ciblée pour la détection de micropolluants émergents dans les boues d'épuration} | Co-encadrement avec Melissa Lopez Viveros, SIAAP\\

& \textbf{Khadija \textsc{Diop}}, Master 2 Systèmes Aquatiques et Gestion de l'Eau, 6 mois. \small\emph{Oxydation de micropolluants organiques en traitement avancé des eaux résiduaires par des procédés d’oxydation} | Encadrement avec Christelle Nabintu Kajoka\\

& \textbf{Elhadji Waly \textsc{Ba}}, Master 2 Quatro, Université de Poitiers, 6 mois. \small\emph{Oxydation de micropolluants organiques en traitement avancé des eaux résiduaires par des procédés d’oxydation} | Encadrement avec Christelle Nabintu Kajoka\\

& \textbf{Salomé \textsc{Dushashvili}}, Master 2 Physico-Chimie moléculaire et applications, Université Gustave Eiffel, 6 mois. \small\emph{Estimation par spectrométrie de masse haute résolution de la toxicité de micropolluants organiques et d’échantillons environnementaux} | Encadrement avec Julien Sade\\

2024 & \textbf{Jeshica \textsc{Thiraimaran}}, Licence 3 Chimie Université Paris-Est Créteil, 2 mois. \small\emph{Faisabilité de l’évaluation de la part de réutilisation indirecte des eaux usées dans la production d’eau potable en France}\\

2025 & \textbf{Lilou \textsc{Chret}}, Licence 3 Chimie-Biologie Université Paris-Est Créteil, 2 mois. \small\emph{Analyse de micropolluants organiques dans des matrices complexes} | Encadrement avec Emilie Caupos\\
}

### Stage doctoral

\twocolsection{}{ 2023 & \textbf{Amina \textsc{Ben Chaaben}}, Doctorante à l'Université du Québec à Rimouski (UQAR), séjour de recherche de 1 mois dans le cadre de sa formation doctorale "Nouveaux Développements en Océanographie". \small\emph{Analyses non-ciblées par spectrométrie de masse haute résolution d'échantillons d'eau du fleuve Saint-Laurent}\\
}

## 2.3 Responsabilités et animations scientifiques

### Animations scientifiques

-   Membre du Comité Scientifique du Leesu depuis 2020, co-animateur d'une des trois thématiques de recherche du laboratoire « Innovations pour la gestion durable de l'eau et de la ville » (organisation de réunions régulières de chercheurs du laboratoire, proposition de séminaires)

-   Gestion du [site internet du laboratoire](https://www.leesu.fr) depuis 2015 (encore épaulé par l'ancien gestionnaire, aujourd'hui retraité) : publication/mise à jour d'articles, gestion du système de contenus, gestion/maintenance du serveur informatique. J'ai notamment entamé une refonte graphique du site, avec sa modernisation (adaptation aux différents formats d'écrans portables).

-   Programme de recherche OPUR : co-animation d'un thème de recherche (R2) de la 5^e^ phase du programme OPUR (2019-2023), et portage de deux actions. Co-animation d'un thème de recherche (R1) de la [6^e^ phase du programme (2024-2029)](https://www.leesu.fr/opur/opur6-2024-2029) et membre du Comité de Coordination du programme. J'ai également pris en charge les aspects liés à la communication et au [site web](https://www.leesu.fr/opur), avec également une refonte graphique intégrale.

-   Co-animateur de l'Axe 2 ("Regarder autrement les eaux de surface") du programme [MeSeine Innovation](#0) (2022-2025) porté par le SIAAP.

-   Membre du comité de pilotage de l'[Observatoire de la Ville](https://inneauvation.fr/decouvrir-inneauvation/observatoires-environnementaux/observatoire-ville-1) (SIAAP) depuis sa création en 2021.

-   Participation à un réseau de recherche : membre du réseau européen NORMAN depuis 2019, dédié à l'analyse et au suivi des micropolluants dans l'environnement (réseau qui organise des essais interlaboratoires à l'échelle européenne, et coordonne plusieurs actions/activités scientifiques/groupes de travail). Participation à plusieurs essais interlaboratoires liés à l'analyse non-ciblée par HRMS.

-   Membre du comité scientifique d'[Hésiode Environnement](https://www.hesiode-environnement.fr/) depuis 2025.

### Organisation de colloques

-   Vice-président de l'Association de Professionnels du Traitement des Eaux et des Nuisances (APTEN Poitiers), organisant tous les deux ans le colloque Journées Information Eaux à Poitiers (500 participants). Membre du comité de sélection scientifique depuis 2018.

-   Membre du comité de pilotage des Journées Scientifiques de l'Environnement, colloque annuel organisé par l'UPEC (OSU-EFLUVE) et le département du Val-de-Marne. Elaboration du programme et animation (2019-2024).

-   Membre du comité scientifique du congrès international du GRUTTEE 2024 (Bordeaux).

### Comités de suivi de thèse, jurys et expertise

#### Comités de suivi

-   **Kevin [Rocco]{.smallcaps}**, « *Stratégies analytiques innovantes pour étudier le devenir des pesticides dans les hydrosystèmes* » -- INRAE/Université de Lyon -- 2019-2022

-   **Karlien [Dejaeger]{.smallcaps}**, « *Risk assessment related to disinfection byproducts formation in drinking water* » -- Université de Ghent et Université de Lille -- 2020-2023

-   **Tom [Ducrocq]{.smallcaps}**, « *Stratégies d'analyses pour l'exploration de la contamination organique des -sédiments de rivières* » -- INRAE/Université de Lyon -- 2021-2024

-   **Mounir [Ayadi]{.smallcaps}**, « *Traitements d'affinage pour le stockage des eaux usées domestiques épurées en vue d'une valorisation en agriculture : Développement d'un traitement d'affinage associant filtration membranaire et couplage UV/chlore pour la réutilisation des eaux usées* » -- Université de Poitiers -- 2022-2025

-   **Armand [Poirier]{.smallcaps}**, « *Usage de la spectroscopie de fluorescence in situ et à haute fréquence pour le suivi de la matière organique dans la file eau et la file boue des STEU : mise en oeuvre d'un outils d'aide à la gestion des procédés* » -- Université Paris-Est Créteil -- 2023-2026

-   **Isabelle [André]{.smallcaps}**, « *Développement de cartes de contrôle multivariées pour le suivi de la qualité des rejets urbains par approche échantillonnage passif et analyses non-ciblées* » -- Ecole Nationale Supérieure de Chimie de Rennes -- 2024-2027

-   **Pierre [Verdieu]{.smallcaps}**, « *Application du plasma froid pour la décontamination chimique et microbiologique des eaux usées* » -- Université de Limoges -- 2024-2027

-   **Ye [Geng]{.smallcaps}**, « *Understanding the ecodynamic of emerging contaminants into the aquatic environment: focus on transformation products* » -- Université de Bordeaux -- 2024-2028

#### Jurys de thèse (examinateur)

-   **Rayana [Manasfi]{.smallcaps}**, « *Uptake of organic micropollutants by vegetable crops irrigated by reclaimed wastewater: Analytical developments to conduct field studies* » -- laboratoire Hydrosciences de l'Université de Montpellier -- soutenue le 24/11/2020

-   **Martin [Maréchal]{.smallcaps}**, « *Caractérisation de la pollution particulaire dans les piscines couvertes à usage collectif* » -- CSTB / Aix-Marseille Université -- soutenue le 22/03/2023

-   **Mohamad [Shalak]{.smallcaps}**, « *Développement de méthodes innovantes pour la caractérisation de la matière organique et de ses produits de transformation dans les filières de potabilisation* » -- Université de Lille -- soutenue le 19/11/2025

-   **Solenne [Reverbel]{.smallcaps}**, « *Apport de la spectrométrie de masse haute résolution pour l'étude des produits de transformation des contaminants émergents* » -- Université de Bordeaux -- soutenue le 09/12/2025

-   **Eloi [Marilleau]{.smallcaps}**, « *Evaluation et validation de concepts de caractérisation de micropolluants organiques en matrices alimentaires et environnementales par le couplage chromatographie liquide-spectrométrie de masse haute résolution* » -- Ecole Nationale Supérieure de Chimie de Rennes -- soutenue le 19/12/2025

#### Comités de sélection - évaluation - expertise

-   Membre du comité de sélection de l'appel à projets Water Research Foundation RFP #4499 - Determine the Relative Importance and Contribution of Anthropogenic and Natural Sources of Nitrosamine Precursors (2013)

-   Evaluation d'un projet ANR JCJC en deuxième phase de l'AAPG 2021 dans le volet "CE45 : Mathématiques et sciences du numérique pour la biologie et la santé"

-   Evaluation d'un projet de recherche ANR JCJC de l'AAPG 2022 dans le volet "CE19 : Technologies pour la santé"

-   Membre du jury du prix de thèse 2022 de l'Association Scientifique et Technique pour l'Eau et l'Environnement (ASTEE).

-   Membre de comités de sélection de recrutement d'enseignants-chercheurs (MCF section 35 FST UPEC 2020, MCF section 35 IUT UPEC 2020, MCF section 62 Université Gustave Eiffel 2020, MCF section 32 Université de Limoges 2021)

-   Evaluation de plusieurs dossiers RIPEC 2022 et 2023

-   Evaluation d'un projet de thèse CIFRE 2025

#### Dissémination

Présentation sur les grands problèmes liés à l'eau et démonstration de traitement d'eau en classe de CP (projet de classe d'eau) à l'Ecole Primaire Simone Veil (Bobigny) (22 mai 2023), et une classe de CM1 à l'Ecole Primaire Sciences et Biodiversité (Boulogne-Billancourt) (30 mai 2024).

### Activité de relecture

Plus d'une centaine de [relecture d'articles](https://www.webofscience.com/wos/author/record/I-6982-2019) dans des journaux à fort facteur d'impact (ex. 24 Water Research, 17 Environmental Science and Pollution Research, 15 Environmental Science & Technology).

\FloatBarrier
\newpage
\fancyhead[CO,CE]{Publications et communications}

# 3. Publications et communications

#### Publications dans des revues internationales à comité de lecture

::: {#refs-papersint}
:::

------------------------------------------------------------------------

#### Publications dans des revues nationales à comité de lecture

::: {#refs-papersnat}
:::

------------------------------------------------------------------------

#### Communications internationales (présentations orales)

::: {#refs-comintorale}
:::

------------------------------------------------------------------------

#### Communications internationales (présentations par affiche)

::: {#refs-comintaff}
:::

------------------------------------------------------------------------

#### Communications nationales (présentations orales)

::: {#refs-comnatorale}
:::

------------------------------------------------------------------------

#### Communications nationales (présentations par affiche)

::: {#refs-comnataff}
:::

------------------------------------------------------------------------

#### Ouvrages - Chapitres d'ouvrage

::: {#refs-chap}
:::

------------------------------------------------------------------------

#### Dépôts de données

::: {#refs-data}
:::

#### Logiciel

::: {#refs-software}
:::

#### Vidéo

::: {#refs-video}
:::
