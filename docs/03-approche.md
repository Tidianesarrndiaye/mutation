# 03 – Approche

> Pistes de réflexion, pas de décisions. Les aspects techniques viendront plus tard.

Public : personnes **sourdes** et **non parlantes**.

## Deux voies

### Voie 1 : inventer un nouveau langage gestuel simple

| Pour | Contre |
|---|---|
| Conçu dès le départ pour ces deux publics | Il faut le créer, l'enseigner et le faire adopter |
| Vocabulaire petit, donc plus facile à reconnaître par une caméra | Une communauté doit l'utiliser : sinon, il ne sert à personne |
| Aucune dépendance aux langues existantes | Les précédents (Makaton, Gestuno…) sont restés marginaux |
| Contrôle total de la grammaire | Les personnes sourdes ont déjà une langue des signes, qu'elles risquent de ne pas vouloir remplacer |

### Voie 2 : langue des signes existante + interprète IA

```
SIGNES  ──caméra──►  IA reconnaissance  ──►  texte / voix        (pour les entendants et les non-parlants)

PAROLE  ──micro───►  IA transcription  ──►  avatar 3D qui signe  (pour les sourds)
```

| Pour | Contre |
|---|---|
| Aucune nouvelle langue à apprendre | Reconnaître des signes en continu est un problème de recherche ouvert |
| Beaucoup de documentation et de jeux de données existent | Les données manquent pour de nombreuses langues des signes (dont africaines) |
| Utile immédiatement aux personnes qui signent déjà | L'avatar doit respecter la grammaire (visage, espace) pour être compris |

### Voie hybride (proposition)

Commencer par la **voie 2**, avec un **petit vocabulaire** de signes très courants (urgence, santé, besoins de base, salutations). Cela réduit la difficulté technique et donne un produit utile. On peut ensuite :

- élargir le vocabulaire ;
- ajouter une couche de **signes simplifiés** là où la reconnaissance échoue ;
- n'inventer un langage (voie 1) que si les tests montrent un vrai besoin.

## Les deux sens à couvrir

| Sens | Entrée | Sortie | Pour qui |
|---|---|---|---|
| Signes → langue vocale | Vidéo (caméra) | Texte et voix de synthèse | Entendants, non-parlants |
| Parole → signes | Audio (micro) | Avatar 3D qui signe + sous-titres | Sourds |

Un utilisateur **sourd et non parlant** utilise le premier sens pour s'exprimer et le second pour comprendre. Un utilisateur **non parlant mais entendant** n'a besoin que du premier.

## Démarche proposée

1. **Choisir la langue des signes** de départ (selon le pays et le public).
2. **Rencontrer des utilisateurs** : sourds, non-parlants, interprètes, familles.
3. **Définir le vocabulaire pilote** (par exemple 50 à 200 signes) pour des scénarios précis.
4. **Étudier les données disponibles** et les besoins de collecte avec des signeurs natifs.
5. **Prototype** : un seul sens d'abord, avec un petit vocabulaire.
6. **Tests avec les utilisateurs**, puis extension du vocabulaire et du second sens.

## Principes

- Impliquer la communauté sourde dès le départ (« rien sur nous sans nous »).
- Se présenter comme une **aide** et non un remplaçant d'interprète.
- Respecter la vie privée : la caméra filme des personnes et des conversations parfois médicales.
- Penser à l'utilisation hors ligne et sur téléphone d'entrée de gamme.

## Risques

| Risque | Réponse |
|---|---|
| Précision insuffisante de la reconnaissance | Petit vocabulaire, retour visuel de ce qui a été compris, correction possible |
| Avatar peu naturel ou incompréhensible | Faire valider par des signeurs natifs |
| Manque de données pour la langue visée | Collecte dédiée, partenariats |
| Conditions réelles (lumière, angle, fond) | Tests terrain précoces |
