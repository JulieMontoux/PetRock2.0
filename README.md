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
| **US-01** | En tant qu'utilisateur, je veux voir mon caillou affiché à l'écran avec un design basique | Must | 3 | 1 | ✅ |
| **US-02** | En tant qu'utilisateur, je veux voir 3 stats (Faim, Ennui, Bonheur) qui diminuent avec le temps | Must | 5 | 1 | ✅ |
| **US-03** | En tant qu'utilisateur, je veux nourrir mon caillou pour restaurer sa Faim | Must | 2 | 1 | ✅ |
| **US-04** | En tant qu'utilisateur, je veux jouer avec mon caillou pour réduire son Ennui | Must | 2 | 1 | ✅ |
| **US-05** | En tant qu'utilisateur, je veux caresser mon caillou pour augmenter son Bonheur | Should | 2 | 1 | ✅ |
| **US-06** | En tant qu'utilisateur, je veux que mon caillou puisse "mourir" (se fissurer) si négligé | Must | 3 | 2 | ⏳ |
| **US-07** | En tant qu'utilisateur, je veux donner un nom à mon caillou | Should | 2 | 2 | ⏳ |
| **US-08** | En tant qu'utilisateur, je veux que mon caillou gagne de l'XP et évolue (Galet → Caillou → Rocher) | Should | 8 | 2 | ⏳ |
| **US-09** | En tant qu'utilisateur, je veux voir des animations quand j'interagis avec le caillou | Could | 5 | 2 | ⏳ |
| **US-10** | En tant qu'utilisateur, je veux voir l'historique des actions sur mon caillou | Won't | 3 | - | ❌ |

**Backlog total : 35 Story Points (hors Won't Have)**

### Répartition des sprints
- **Sprint 1 (90 min)** : 14 pts — Caillou vivant avec besoins de base ✅ **100% LIVRÉ**
- **Sprint 2 (90 min)** : 13-18 pts — Progression, gamification et mort du caillou

---

## Sprint 1 — Ce qui a été livré ✅

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

## Sprint 2 — Ce qui a été livré
*[À compléter après le sprint]*

**Fonctionnalités démo-ables :**
- 
- 
- 

**Vélocité réelle : ___ pts sur 13 pts prévus**

---

## Ce qui a été reporté et pourquoi

| User Story | Raison du report |
|---|---|
| *Aucune US reportée du Sprint 1* | Sprint 1 livré à 100% 🎉 |

---

## Notre Burn-up Chart
*[Mis à jour après Sprint 1]*
```
Story Points
35 │                              ┌─────  Scope total (35 pts)
30 │                             ╱
25 │                            ╱
20 │                           ╱
15 │                          ╱
14 │         ●───────────────╱   ← Sprint 1 : 14 pts livrés (100%)
10 │        ╱               ╱
 5 │       ╱               ╱
 0 │______╱_______________╱____________
        S1              S2         S3 (proj.)
```

**Vélocité Sprint 1 : 14 pts | Sprint 2 : ___ pts**

**Projection :** Avec une vélocité de 14 pts/sprint, nous sommes en capacité de livrer 28 pts sur 2 sprints (80% du scope total). Si Sprint 2 maintient cette vélocité, nous livrerons toutes les US Must Have + Should Have prioritaires.

---

## Nos décisions techniques

**Stack choisie :** 
- **Frontend** : HTML/CSS/JavaScript Vanilla
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

---

## Comment on a utilisé l'IA

**Prompts qui ont bien marché :**
- "Génère un système de stats pour un Tamagotchi en JS vanilla avec decay automatique basé sur le temps écoulé"
- "Crée un SVG de caillou mignon style cartoon avec des yeux et un petit sourire"
- "Comment sauvegarder et récupérer un objet JavaScript dans LocalStorage ?"
- "Fais-moi une animation CSS de cœur qui apparaît puis disparaît en 1 seconde"
- "Debug : pourquoi mon setInterval ne se lance pas au chargement de la page ?"

**Ce que l'IA n'a pas su faire :**
- Choisir les bonnes valeurs de decay et de restauration (on a dû tester et ajuster plusieurs fois)
- Créer un design de caillou qui soit "absurde mais attachant" (beaucoup d'itérations)
- Comprendre qu'on voulait que le temps continue de s'écouler même quand la page est fermée (on a dû reformuler)

**Temps gagné estimé :** ~1h sur le setup HTML/CSS/JS et les animations

---

## Rétrospective Sprint 1

| | Sprint 1 |
|---|---|
| ✓ **Ce qui a marché** | - **Vélocité parfaite** : 14/14 pts livrés, aucune US reportée<br>- **Collaboration fluide** : Tous les membres ont commité, bonnes PR reviews<br>- **L'IA a vraiment aidé** : Gain de temps sur le boilerplate et les animations CSS<br>- **LocalStorage impeccable** : Fonctionne du premier coup après ajustements<br>- **Stand-up efficace** : On a détecté un bug tôt et corrigé immédiatement |
| △ **Ce qu'on améliorerait** | - **Estimation trop prudente ?** On a fini 15 min en avance, on aurait pu prendre US-07 (nom du caillou)<br>- **Tests manuels** : On n'a testé la persistance qu'à la fin, il fallait le faire plus tôt<br>- **Messages de commit** : Quelques commits pas assez descriptifs (ex: "fix bug" au lieu de "fix: stats not updating correctly") |
| 🎯 **Action items pour Sprint 2** | - **Être plus ambitieux** : Si on termine en avance, prendre une US Should Have du backlog<br>- **Tester au fur et à mesure** : Chaque feature testée immédiatement après merge<br>- **Meilleurs commits** : Respecter strictement le format conventionnel (feat:/fix:/docs:)<br>- **Découper US-08** : L'US évolution (8 pts) doit être découpée en sous-tâches |

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
- Temps moyen avant que le caillou "meure" : ~10 minutes sans interaction (volontairement court pour tester rapidement)
- Nombre de fois où on s'est demandé "mais pourquoi un caillou a faim ?" : 37
- Probabilité qu'un combat de cailloux ait du sens : 0%
- Stack technique : Le strict minimum pour qu'un caillou soit heureux

*Made with ❤️ and complete absurdity*