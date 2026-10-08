# 02 – Solutions existantes

> État de l'art établi à partir de connaissances générales. Les noms, offres et fonctionnalités **(à vérifier)** avant toute décision : ce domaine évolue vite.

## 1. Transcription de la parole en texte (entendant → sourd)

| Solution | Principe | Limites |
|---|---|---|
| Google Live Transcribe / Live Caption | Sous-titres en temps réel sur Android | Texte seulement, qualité variable (bruit, accents, langues peu dotées) |
| Apple Live Captions / Live Listen | Idem sur iOS | Idem, écosystème fermé |
| Ava, Otter, sous-titrage Teams / Meet / Zoom | Sous-titres de conversations et réunions | Dépend du texte écrit ; pas pensé pour les signeurs |
| Services de relais (téléphone sous-titré, relais vidéo avec interprète) | Un humain fait le pont | Coût, disponibilité, inexistant dans beaucoup de pays |

## 2. Communication alternative et améliorée – CAA (personnes non parlantes)

| Solution | Principe | Limites |
|---|---|---|
| Proloquo2Go, TD Snap, Grid 3, LAMP Words for Life, Avaz | Grilles de symboles → voix de synthèse | Surtout pour un locuteur non parlant face à un entendant ; payant ; peu pensé pour la surdité |
| Cboard | Application CAA **open source** | Idem, peu de langues africaines |
| Banques de pictogrammes : **ARASAAC**, Widgit, PCS, Bliss, Makaton | Symboles standardisés | Licences variables (ARASAAC : CC BY-NC-SA) ; l'expressivité reste limitée |
| Voiceitt, Project Relate (Google) | Reconnaissance des paroles atypiques | Concerne les voix atypiques, pas l'absence de voix |

## 3. Langue des signes → texte/voix (reconnaissance)

| Solution | Principe | Limites |
|---|---|---|
| SignAll, KinTrans, Sign-Speak | Reconnaissance de signes par caméra / IA | Souvent une seule langue (ASL), vocabulaire restreint, produits propriétaires |
| Gants connectés (recherche UCLA 2020, Enable Talk…) | Capteurs sur la main | Ne captent pas le visage ni le corps ; **rejetés par une large partie de la communauté sourde** ; peu pratiques |
| Recherche : MediaPipe / OpenPose, datasets WLASL, How2Sign, RWTH-PHOENIX-2014T | Estimation de pose + modèles séquentiels/transformers | Reconnaissance de **mots isolés** plutôt que traduction continue ; données rares |

## 4. Texte/voix → langue des signes (génération)

| Solution | Principe | Limites |
|---|---|---|
| Hand Talk (Libras, Brésil), avatars 3D | Avatar qui signe un texte | Traduction littérale, expressions du visage limitées, accueil mitigé |
| Signapse, vidéos de signeurs générées par IA | Rendu photoréaliste | Qualité de la grammaire à valider par la communauté |
| Sign.mt (open source) | Texte ↔ signes dans le navigateur | Prototype de recherche, couverture limitée |

## 5. Messagerie visuelle et émojis

- Les émojis et stickers sont déjà un « langage commun » informel, mais sans grammaire et ambigus.
- Aucune solution grand public ne les structure en véritable langage pivot pour ce public.

## Synthèse : ce qui manque

1. **Peu de solutions couvrent le cas « sourd ↔ non parlant »** : les outils sont conçus pour un seul handicap à la fois.
2. **Pas de langage pivot partagé** : chaque outil convertit un canal en un autre (parole → texte, symboles → voix), rarement les trois.
3. **Couverture linguistique** : très peu de solutions pour les langues des signes africaines ou pour des langues vocales comme le wolof.
4. **Dépendance au texte** : exclut les personnes peu lettrées, dont une partie des sourds de naissance.
5. **Coût et connectivité** : beaucoup d'outils sont payants, en ligne ou réservés à certains appareils.

## Critiques récurrentes de la communauté sourde

- La Fédération mondiale des sourds (WFD) et des associations nationales ont critiqué les « gants traducteurs » et les avatars quand ils prétendent remplacer les interprètes.
- Une langue des signes ne se réduit pas aux mains : visage, regard, posture et espace comptent.
- Les jeux de données sont souvent construits sans signeurs natifs.

Conséquence pour Mutation : se positionner comme un **outil d'aide à la communication** et non comme un remplaçant d'interprète, et valider avec les utilisateurs à chaque étape.
