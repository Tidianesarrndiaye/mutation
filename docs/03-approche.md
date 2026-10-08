# 03 – Approche

> Pistes de réflexion, pas de décisions. Les aspects techniques viendront plus tard.

## Idée centrale

Construire un **langage pivot** : une représentation commune dans laquelle chaque interlocuteur écrit/signe/montre dans son mode préféré, et reçoit dans le sien.

```
 Parole ─┐                         ┌─ Sous-titres / texte
 Texte ──┤                         ├─ Voix de synthèse
 Signes ─┼──►  Langage pivot  ──►──┼─ Pictogrammes
 Pictos ─┘   (sens, intention)     └─ Avatar signeur
```

## Options pour le langage pivot

| Option | Avantages | Inconvénients |
|---|---|---|
| **A. Pictogrammes / symboles** | Accessible aux non-lecteurs, offline possible, banques existantes (ARASAAC) | Vocabulaire limité, expression abstraite et nuancée difficile |
| **B. Texte** | Simple, couvert par les modèles de langue | Exclut les non-lecteurs ; pas la langue première de beaucoup de sourds |
| **C. Langue des signes** | Naturelle pour les sourds signeurs | Techniquement très difficile ; données rares ; plusieurs langues |
| **D. Hybride** : pictos + texte + voix, signes en second temps | Couvre plus de profils, livrable par étapes | Plus de travail de conception |

**Recommandation de départ** : option **D**, en commençant par A + B (faisables vite) et en gardant C pour une phase ultérieure.

## Démarche proposée

1. **Comprendre les utilisateurs** : entretiens avec des personnes sourdes, non parlantes, des familles, des enseignants, des interprètes.
2. **Choisir un contexte pilote** : une langue, un lieu (école spécialisée, centre de santé…) et quelques scénarios réels.
3. **Prototype papier / maquettes** : tester le langage pivot sans code (cartes, tableaux de symboles, Wizard of Oz).
4. **MVP minimal** : conversation à deux, pictogrammes + texte + voix, utilisable hors ligne.
5. **Extension** : reconnaissance de signes, avatar, nouvelles langues.
6. **Évaluation continue** avec les utilisateurs.

## Principes de conception

- **Accessibilité d'abord** : grands boutons, contrastes, retours visuels, vibrations, pas de dépendance au son.
- **Hors ligne par défaut** si possible (connectivité limitée).
- **Respect de la vie privée** : les conversations touchent à la santé et à la vie privée ; limiter les données stockées.
- **Co-conception** avec la communauté et honnêteté sur les limites de l'outil.
- **Open source** envisageable pour faciliter l'adoption et les contributions (à discuter).

## Risques

| Risque | Piste de réponse |
|---|---|
| Langage pivot mal compris par les utilisateurs | Prototypage précoce et tests terrain |
| Manque de données (signes locaux) | Collecte avec consentement et signeurs natifs, partenariats |
| Promesses excessives (« traduction parfaite ») | Communication prudente, mention des limites |
| Fragmentation des langues | Démarrer par une langue et un contexte |
