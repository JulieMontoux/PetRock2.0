# PetRock2.0
Tamagotchi de caillou - Parce que votre caillou mérite de l'amour (et qu'il a faim, allez savoir pourquoi).

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
| **US-01** | En tant qu'utilisateur, je veux voir mon caillou affiché à l'écran avec un design basique | Must | 3 | 1 | ⏳ |
| **US-02** | En tant qu'utilisateur, je veux voir 3 stats (Faim, Ennui, Bonheur) qui diminuent avec le temps | Must | 5 | 1 | ⏳ |
| **US-03** | En tant qu'utilisateur, je veux nourrir mon caillou pour restaurer sa Faim | Must | 2 | 1 | ⏳ |
| **US-04** | En tant qu'utilisateur, je veux jouer avec mon caillou pour réduire son Ennui | Must | 2 | 1 | ⏳ |
| **US-05** | En tant qu'utilisateur, je veux caresser mon caillou pour augmenter son Bonheur | Should | 2 | 1 | ⏳ |
| **US-06** | En tant qu'utilisateur, je veux que mon caillou puisse "mourir" (se fissurer) si négligé | Must | 3 | 2 | ⏳ |
| **US-07** | En tant qu'utilisateur, je veux donner un nom à mon caillou | Should | 2 | 2 | ⏳ |
| **US-08** | En tant qu'utilisateur, je veux que mon caillou gagne de l'XP et évolue (Galet → Caillou → Rocher) | Should | 8 | 2 | ⏳ |
| **US-09** | En tant qu'utilisateur, je veux voir des animations quand j'interagis avec le caillou | Could | 5 | 2 | ⏳ |
| **US-10** | En tant qu'utilisateur, je veux voir l'historique des actions sur mon caillou | Won't | 3 | - | ❌ |

**Backlog total : 35 Story Points (hors Won't Have)**

### Répartition des sprints
- **Sprint 1 (90 min)** : 14 pts — Caillou vivant avec besoins de base
- **Sprint 2 (90 min)** : 13-18 pts — Progression, gamification et mort du caillou

---

## Sprint 1 — Ce qui a été livré
*[À compléter après le sprint]*

**Fonctionnalités démo-ables :**
- 
- 
- 

**Vélocité réelle : ___ pts sur 14 pts prévus**

---

## Sprint 2 — Ce qui a été livré
*[À compléter après le sprint]*

**Fonctionnalités démo-ables :**
- 
- 
- 

**Vélocité réelle : ___ pts sur 13 pts prévus**

---

## Ce qui a été reporté et pourquoi
*[À compléter en fin de projet]*

| User Story | Raison du report |
|---|---|
| | |

---

## Notre Burn-up Chart
*[À générer après chaque sprint avec vos vraies données]*

```
Story Points
35 │                    ┌─────  Scope total (35 pts)
30 │                   ╱
25 │                  ╱
20 │                 ╱
15 │           ?    ╱
10 │          ╱    ╱
 5 │    ?   ╱    ╱
 0 │___╱________╱____________
     S1      S2      S3 (proj.)
```

**Vélocité Sprint 1 : ___ pts | Sprint 2 : ___ pts**

---

## Nos décisions techniques

**Stack choisie :** 
- **Frontend** : HTML/CSS/JavaScript Vanilla
- **Style** : CSS pur avec animations
- **Stockage** : LocalStorage uniquement (pas de backend)
- **Déploiement** : GitHub Pages ou Netlify

**Pourquoi :**
- Simplicité maximale pour tenir les 2 sprints de 90 min
- Pas de configuration complexe ni de dépendances lourdes
- 100% frontend = déployable en 1 clic
- LocalStorage suffit pour un Tamagotchi solo

**1 décision d'architecture importante :**
Système de **tick automatique** avec `setInterval(updateStats, 30000)` (toutes les 30s) qui fait décrémenter les stats. Sauvegarde auto dans LocalStorage à chaque action pour persister l'état même si l'utilisateur ferme l'onglet. Le timer se base sur `Date.now()` pour calculer le temps écoulé et rattraper les stats si l'app est fermée puis rouverte.

---

## Comment on a utilisé l'IA

**Prompts qui ont bien marché :**
- *[À documenter pendant le projet]*
- 
- 

**Ce que l'IA n'a pas su faire :**
- *[À documenter]*
- 

**Temps gagné estimé :** ___ heures

---

## Rétrospective finale

| | Sprint 1 | Sprint 2 |
|---|---|---|
| ✓ **Ce qui a marché** | *[À compléter]* | *[À compléter]* |
| △ **Ce qu'on améliorerait** | *[À compléter]* | *[À compléter]* |
| 🎯 **Action items** | *[À compléter]* | *[À compléter]* |

---

## Lancer le projet en local

```bash
# Clone le repo
git clone https://github.com/JulieMontoux/PetRock2.0.git

# Ouvre simplement index.html dans ton navigateur
open index.html
# ou double-clic sur le fichier
```

---

**🪨 Fun Facts du Projet :**
- Temps moyen avant que le caillou "meure" : ~90 minutes sans interaction
- Nombre de façons de nourrir un caillou imaginées : 7 (graviers, eau, compliments, soleil...)
- Probabilité qu'un combat de cailloux ait du sens : 0%
- Stack technique : Le strict minimum pour qu'un caillou soit heureux

*Made with ❤️ and complete absurdity*