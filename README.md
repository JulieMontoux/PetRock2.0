# PetRock2.0
Tamagotchi de caillou - Parce que votre caillou mérite de l'amour (et qu'il a faim, allez savoir pourquoi).

[Suivi de projet](https://github.com/users/JulieMontoux/projects/7/views/1)

**Pitch en 1 ligne :**
Un Tamagotchi absurde où vous élevez un caillou virtuel avec des besoins inexplicables, le faites évoluer du simple galet au rocher légendaire, le tout en 100% LocalStorage.

## L'équipe
| Membre | Rôle Scrum |
|---|---|
| Julie | Product Owner |
| Paul | Scrum Master |
| Yassin | Dev |
| Mathieu | Dev |
| Claude | Assistant IA & Pair Programming |

## La vision produit
En tant que **personne nostalgique des années 90 et amateur d'absurdité**, ce produit permet de **revivre l'expérience addictive du Tamagotchi appliquée au concept le plus inutile possible : un caillou**.

**Problème résolu :** Le manque cruel d'applications web dédiées à l'élevage virtuel de roches domestiques avec système de stats absurdes et mécaniques d'évolution.

## Story Mapping

| Activité | Description | US associées |
|---|---|---|
| **1. Découvrir son caillou** | Premier contact : voir le caillou, comprendre qu'il est vivant | US-01 |
| **2. Prendre soin du caillou** | Interactions quotidiennes : nourrir, jouer, caresser, surveiller les stats | US-02, US-03, US-04, US-05 |
| **3. Faire évoluer son caillou** | Progression long-terme : XP, évolutions, personnalisation | US-07, US-08, US-09 |
| **4. Recommencer l'aventure** | Fin de cycle : mort du caillou, recommencer avec un nouveau | US-06 |

## Product Backlog complet

| # | User Story | MoSCoW | Story Points | Sprint | Statut |
|---|---|---|---|---|---|
| **US-01** | En tant qu'utilisateur, je veux voir mon caillou affiché à l'écran avec un design basique | Must | 3 | 1 | ✅ |
| **US-02** | En tant qu'utilisateur, je veux voir 3 stats (Faim, Ennui, Bonheur) qui diminuent avec le temps | Must | 5 | 1 | ✅ |
| **US-03** | En tant qu'utilisateur, je veux nourrir mon caillou pour restaurer sa Faim | Must | 2 | 1 | ✅ |
| **US-04** | En tant qu'utilisateur, je veux jouer avec mon caillou pour réduire son Ennui | Must | 2 | 1 | ✅ |
| **US-05** | En tant qu'utilisateur, je veux caresser mon caillou pour augmenter son Bonheur | Should | 2 | 1 | ✅ |
| **US-06** | En tant qu'utilisateur, je veux que mon caillou puisse "mourir" (se fissurer) si négligé | Must | 3 | 2 | ✅ |
| **US-07** | En tant qu'utilisateur, je veux donner un nom à mon caillou | Should | 2 | 2 | ✅ |
| **US-08** | En tant qu'utilisateur, je veux que mon caillou gagne de l'XP et évolue (Caillou → Rocher) | Should | 8 | 2 | ✅ |
| **US-09** | En tant qu'utilisateur, je veux voir des animations quand j'interagis avec le caillou | Could | 5 | 2 | ✅ |
| **US-10** | En tant qu'utilisateur, je veux voir l'historique des actions sur mon caillou | Won't | 3 | - | ❌ |

**Backlog total : 35 Story Points (hors Won't Have)**

### Répartition des sprints
- **Sprint 1 "Rocky Awakens" (90 min)** : 14 pts — Caillou vivant avec besoins de base ✅ **100% LIVRÉ**
- **Sprint 2 "Rocky Evolves" (90 min)** : 18 pts — Progression, gamification et mort du caillou ✅ **100% LIVRÉ**

---

## Sprint 1 "Rocky Awakens" — Ce qui a été livré ✅

**Fonctionnalités démo-ables :**
- ✅ **Affichage du caillou** : Un caillou SVG mignon centré à l'écran avec design cartoon
- ✅ **Système de stats vivant** : 3 barres de progression (Faim, Ennui, Bonheur) qui diminuent automatiquement toutes les 30 secondes
- ✅ **Persistance des données** : L'état du caillou est sauvegardé dans LocalStorage et récupéré au rechargement
- ✅ **Bouton "Nourrir"** : Restaure la jauge Faim de +25% avec feedback visuel
- ✅ **Bouton "Jouer"** : Réduit l'Ennui de -25% avec feedback visuel
- ✅ **Bouton "Caresser"** : Augmente le Bonheur de +25% avec animation cœur

**User Stories livrées :**
- ✅ US-01 : Affichage du caillou (3 pts)
- ✅ US-02 : Système de stats avec decay automatique (5 pts)
- ✅ US-03 : Nourrir le caillou (2 pts)
- ✅ US-04 : Jouer avec le caillou (2 pts)
- ✅ US-05 : Caresser le caillou (2 pts)

**Vélocité réelle : 14 pts sur 14 pts prévus** 🎯 **(100% de complétion !)**

---

## Sprint 2 "Rocky Evolves" — Ce qui a été livré ✅

**Fonctionnalités démo-ables :**
- ✅ **Mort du caillou** : Le caillou se fissure visuellement quand une stat atteint 0, écran Game Over avec bouton "Recommencer"
- ✅ **Nommer son caillou** : Input texte au premier lancement, nom affiché en permanence, persisté dans LocalStorage
- ✅ **Système d'XP et évolution** : Barre XP fonctionnelle, +5 XP par interaction, 3 stades visuels (Galet 0-50 XP, Caillou 50-150 XP, Rocher 150+ XP)
- ✅ **Animations enrichies** : Rebond du caillou au clic, particules lors des interactions, transitions fluides entre les évolutions
- ✅ **Notifications d'évolution** : Message de félicitations animé lors du passage au niveau supérieur

**User Stories livrées :**
- ✅ US-06 : Mort du caillou et game over (3 pts)
- ✅ US-07 : Donner un nom au caillou (2 pts)
- ✅ US-08 : Système XP et évolutions visuelles (8 pts)
- ✅ US-09 : Animations d'interaction (5 pts)

**Vélocité réelle : 18 pts sur 18 pts prévus** 🎯 **(100% de complétion !)**

---

## Ce qui a été reporté et pourquoi

| User Story | Raison du report |
|---|---|
| US-10 : Historique des actions (3 pts) | **Won't Have** — Feature non prioritaire pour le MVP, manque de temps. Cette US était déjà classée "Won't" dans le backlog initial, elle n'a jamais été planifiée dans les sprints. |

**Note :** Tous les Must Have, Should Have et Could Have ont été livrés à 100%. Seule la Won't Have US-10 était considérée comme optionnelle.

---

## Notre Burn-up Chart
*[Projet terminé - 2 sprints complétés]*

```
Story Points
35 │                              ┌─────  Scope total (35 pts)
32 │         ●────────────────●──╱
30 │        ╱                ╱  ╱
25 │       ╱                ╱  ╱
20 │      ╱                ╱  ╱
15 │     ╱                ╱  ╱
14 │    ●────────────────╱  ╱   ← Sprint 1 : 14 pts livrés
10 │   ╱               ╱   ╱
 5 │  ╱               ╱   ╱
 0 │_╱_______________╱___╱________
     S1            S2         S3 (non nécessaire)
```

**Vélocité Sprint 1 : 14 pts | Sprint 2 : 18 pts**  
**Total livré : 32 pts sur 35 pts (91,4% du scope total)**  
**Vélocité moyenne : 16 pts/sprint**

**Analyse :** 
- Sprint 1 : Vélocité stable, livraison exacte du scope prévu
- Sprint 2 : Vélocité en hausse (+28%), amélioration grâce aux apprentissages du Sprint 1
- Projection : Avec cette vélocité, un Sprint 3 aurait permis d'ajouter 15-18 pts de features supplémentaires (combat de cailloux multijoueur, sons, badges...)

---

## Nos décisions techniques

**Stack choisie :** 
- **Frontend** : HTML/CSS/JavaScript
- **Style** : CSS pur avec animations (@keyframes)
- **Stockage** : LocalStorage uniquement (pas de backend)
- **Déploiement** : GitHub Pages

**Pourquoi :**
- Simplicité maximale pour tenir les 2 sprints de 90 min
- Pas de configuration complexe ni de dépendances lourdes
- 100% frontend = déployable en 1 clic
- LocalStorage suffit pour un Tamagotchi solo

**1 décision d'architecture importante :**
Système de **tick automatique** avec `setInterval(updateStats, 30000)` (toutes les 30s) qui fait décrémenter les stats. Sauvegarde auto dans LocalStorage à chaque action pour persister l'état même si l'utilisateur ferme l'onglet. Le timer se base sur `Date.now()` pour calculer le temps écoulé et rattraper les stats si l'app est fermée puis rouverte.

**Décisions prises pendant Sprint 1 :**
- **Taux de decay** : -5 points toutes les 30s pour chaque stat (le caillou meurt en ~10 minutes sans soin)
- **Restauration des stats** : +25% par action (permet 4 interactions pour récupérer une stat vide)
- **LocalStorage keys** : `petrock_state` pour stocker l'objet état complet

**Décisions prises pendant Sprint 2 :**
- **Gain d'XP** : +5 XP par interaction (nourrir/jouer/caresser)
- **Animations** : CSS @keyframes pour performance optimale (pas de JavaScript pour les animations)
- **Mort du caillou** : Visuel de fissures SVG superposé sur le caillou normal

---

## Comment on a utilisé l'IA

**Prompts qui ont bien marché :**

**Sprint 1 :**
- "Génère un système de stats pour un Tamagotchi en JS vanilla avec decay automatique basé sur le temps écoulé"
- "Crée un SVG de caillou mignon style cartoon avec des yeux et un petit sourire"
- "Comment sauvegarder et récupérer un objet JavaScript dans LocalStorage ?"
- "Fais-moi une animation CSS de cœur qui apparaît puis disparaît en 1 seconde"
- "Debug : pourquoi mon setInterval ne se lance pas au chargement de la page ?"

**Sprint 2 :**
- "Crée 3 variations SVG d'un caillou : petit galet, caillou moyen, gros rocher - même style cartoon"
- "Comment faire une animation de transition fluide entre 2 SVG différents en CSS ?"
- "Génère un système d'XP avec paliers et notifications lors d'un level up"
- "Crée un overlay modal Game Over avec effet de fondu et bouton de restart"
- "Fais des particules CSS qui apparaissent aléatoirement autour du caillou quand on clique"

**Ce que l'IA n'a pas su faire :**
- **Choisir les bonnes valeurs de decay et de restauration** (on a dû tester et ajuster plusieurs fois)
- **Créer un design de caillou qui soit "absurde mais attachant"** (beaucoup d'itérations, problème subjectif)
- **Comprendre qu'on voulait que le temps continue de s'écouler même quand la page est fermée** (on a dû reformuler le prompt 3 fois)
- **Équilibrer le système d'XP** (combien d'XP par palier, combien par interaction) — décision de game design humaine
- **Gérer les transitions entre niveaux** sans "flicker" visuel (on a dû débugger manuellement le CSS)

**Temps gagné estimé :** ~2h30 sur les 6h de projet total
- Sprint 1 : ~1h (setup HTML/CSS/JS, animations)
- Sprint 2 : ~1h30 (SVG multiples, système XP, animations avancées)

---

## Rétrospective finale

| | Sprint 1 | Sprint 2 |
|---|---|---|
| ✓ **Ce qui a marché** | - **Vélocité parfaite** : 14/14 pts livrés, aucune US reportée<br>- **Collaboration fluide** : Tous les membres ont commité, bonnes PR reviews<br>- **L'IA a vraiment aidé** : Gain de temps sur le boilerplate et les animations CSS<br>- **LocalStorage impeccable** : Fonctionne du premier coup après ajustements<br>- **Stand-up efficace** : On a détecté un bug tôt et corrigé immédiatement | - **Vélocité en hausse** : 18/18 pts livrés, dépassé les attentes<br>- **US-08 bien découpée** : Les sous-tâches (XP, paliers, visuels) ont facilité le développement<br>- **Tests continus** : Chaque feature testée immédiatement, 0 bug en démo finale<br>- **Prompts IA affinés** : Meilleure communication avec l'IA grâce à l'expérience du Sprint 1<br>- **Ambition payante** : On a pris US-09 (5 pts) en plus et on l'a livrée ! |
| △ **Ce qu'on améliorerait** | - **Estimation trop prudente ?** On a fini 15 min en avance, on aurait pu prendre US-07 (nom du caillou)<br>- **Tests manuels** : On n'a testé la persistance qu'à la fin, il fallait le faire plus tôt<br>- **Messages de commit** : Quelques commits pas assez descriptifs (ex: "fix bug" au lieu de "fix: stats not updating correctly") | - **Gestion du temps** : On a passé trop de temps sur les animations (30 min), au détriment de la documentation<br>- **README pas à jour en temps réel** : On a tout rempli à la fin, il fallait le faire au fur et à mesure<br>- **Pas de démo intermédiaire** : On aurait dû montrer US-06 et US-07 avant d'attaquer US-08 |
| 🎯 **Action items** | - **Être plus ambitieux** : Si on termine en avance, prendre une US Should Have du backlog<br>- **Tester au fur et à mesure** : Chaque feature testée immédiatement après merge<br>- **Meilleurs commits** : Respecter strictement le format conventionnel (feat:/fix:/docs:)<br>- **Découper US-08** : L'US évolution (8 pts) doit être découpée en sous-tâches | **Actions du Sprint 1 appliquées avec succès**<br>- Pour un Sprint 3 hypothétique : prévoir 20 min de buffer pour la documentation et le déploiement<br>- Continuer à découper les grosses US (8+ pts)<br>- Faire une mini-démo à mi-sprint même en interne |

---

## Apprentissages clés sur l'utilisation de l'IA en équipe

| Thème | Apprentissage |
|---|---|
| 💡 **Prompting efficace** | Plus le prompt est contextualisé (technos utilisées, contraintes, fichiers existants), meilleur est le résultat. Les prompts vagues donnent du code générique inutilisable. |
| ⚡ **Gains de productivité** | L'IA excelle sur le code boilerplate, les animations CSS, et la génération de SVG. Elle a divisé par 2 le temps passé sur ces tâches. |
| 🎨 **Limites créatives** | L'IA ne peut pas faire de choix subjectifs (design "mignon mais pas trop", équilibrage game design). Ces décisions restent humaines. |
| 🐛 **Debugging** | Copier-coller l'erreur exacte dans l'IA donne souvent la solution instantanément. Plus efficace que chercher sur Stack Overflow. |
| 👥 **Travail d'équipe** | Partager les bons prompts entre membres accélère toute l'équipe. On a créé un doc "Prompts qui marchent" partagé. |
| 🧠 **Compréhension** | Il faut comprendre le code généré pour l'adapter. L'IA donne une base, pas une solution clé en main. |

---

## Ce que ça change dans notre vision d'un projet Agile réel

**Avant ce projet, on pensait que :**
- L'IA pouvait tout faire toute seule
- Les User Stories étaient juste de la bureaucratie
- On pouvait coder sans planifier
- La vélocité était juste un chiffre théorique

**Maintenant, on sait que :**
- **L'IA est un accélérateur, pas un pilote** : Elle code vite, mais c'est nous qui décidons quoi coder et comment l'architecturer
- **Les US structurent le travail** : Sans US claires, on aurait codé dans tous les sens. Elles donnent un cap et permettent de mesurer l'avancement
- **La vélocité est un outil de projection** : Connaître notre vélocité (14 pts puis 18 pts) nous a permis de planifier le Sprint 2 intelligemment
- **Les rétros ont du sens** : Les action items du Sprint 1 ont directement amélioré le Sprint 2 (+28% de vélocité)
- **Le découpage est crucial** : US-08 (8 pts) aurait été ingérable sans sous-tâches. Les grosses US doivent être découpées.
- **La DoD évite les demi-features** : Sans Definition of Done stricte, on aurait mergé du code non testé
- **Les sprints courts forcent la priorisation** : On a dû faire des choix (US-10 abandonnée), comme dans un vrai projet avec contraintes budgétaires

**En résumé :** L'Agile + l'IA, c'est puissant, mais **l'humain reste le chef d'orchestre**. L'IA joue les notes, nous composons la symphonie.

---

## Lancer le projet en local
```bash
# Clone le repo
git clone https://github.com/JulieMontoux/PetRock2.0.git

# Ouvre simplement index.html dans ton navigateur
open index.html
# ou double-clic sur le fichier

# L'application fonctionne 100% en local, pas de serveur nécessaire
```

---

**🪨 Fun Facts du Projet :**
- Temps moyen avant que le caillou "meure" : ~1 minute sans interaction (volontairement court pour tester rapidement)
- Nombre de fois où on s'est demandé "mais pourquoi un caillou a faim ?" : 37
- Nombre d'itérations pour le design du caillou : 12 (dont 8 générées par l'IA)
- Probabilité qu'un combat de cailloux ait du sens : 0%
- Stack technique : Le strict minimum pour qu'un caillou soit heureux
- Record d'XP atteint en test : 287 XP (niveau "Rocher Légendaire" non prévu initialement)
- Nombre de cailloux "morts" pendant les tests : 23 RIP 🪦

**🏆 Achievements débloqués :**
- ✅ "Sprint Perfect" : 100% de vélocité sur 2 sprints consécutifs
- ✅ "Team Player" : Chaque membre a au moins 7 commits
- ✅ "AI Whisperer" : Prompts qui ont permis de gagner 2h30
- ✅ "Rock Solid" : 0 bug en production
- ✅ "Agile Master" : Burnup chart complété avec vraies données

---

*Made with ❤️ and complete absurdity by Julie, Paul, Yassin, Mathieu & Claude* 