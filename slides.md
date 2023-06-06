---
marp: true
theme: uncover
---

<!-- proposal: https://gospeak.io/u/talks/code-legacy-les-cles-pour-s-en-sortir -->

# **Code legacy 🧟**

Les clés pour s'en sortir !

<style>
blockquote {
  font-size: 120%;
  margin: 0.8em 0;
}
</style>

<!--

PLAN

- Le code legacy (2mn)
- Pistes et écueils typiques ⇒ clés: (3mn)
- Étude de cas: (4mn)
- Take-aways: (1mn)
    - Devs ET entreprise ont **intérêt à maitriser** la complexité accidentelle de leur code
    - **Prioriser les problèmes** en fonction des coûts & risques induits ET de la direction stratégique de l’entreprise
    - **Convaincre** sur la base d’un **plan** avec objectifs mesurables
    - Avancer **progressivement**, en rassurant les personnes impactées

-->

---

> "Legacy Code is **valuable** code you’re **afraid** to change"

Nicolas Carlo & Alex Bolboaca

<!-- notion de peur mais aussi de valeur pour l'entreprise -->

---

## **Symptomes** de code legacy

* 👼 Devs *irremplaçables*

* 😅 Délais et/ou craintes

* 🫣 Recrutement difficile

* 🥵 Bugs et regressions

---

## Problèmes pour les **dévs**

1. 😓 Rechignement

2. 😤 Tensions

3. 🙈 Résignation

---

## Problèmes pour l’**entreprise** 🏭

- 📉 Perte de compétitivité

- 👋 Churn

- ⚰️ “bus factor” 

---

## ❌ Refonte sans fin

* ➡️ planification et accompagnement à prévoir

---

## ❌ Pas le temps / pas le budget

* ➡️ risques et/ou coûts à présenter

---

## ❌ Refonte furtive

* ➡️ **confiance** à recréer entre équipes

<!--
Raisons de ne pas le faire:
- perte de confiance: PM et/ou direction
- deux codebases à maintenir 🥵
- risque de refonte avortée
    - ex: codebase laissée dans un état encore pire
-->

---

📌 ÉTUDE DE CAS

---

## Problème

<!--
- [problème] équipe tech a du mal à maitriser la complexité croissante du code produit ⇒ bugs, regressions et coût d’onboarding 🥵
- [coordination] équipe produit veut internationaliser son app e-commerce, pour que les clients commandent depuis FR et USA 🌠
- [priorisation] équipe tech prévient que le code sous-jacent est fragile ⇒ risque de bugs, regressions et/ou retards sur la livraison 💣
- [plan] refonte du “checkout”, de manière à le rendre agnostique de la devise et des prestataires de livraison 🏗️
    - ⇒ réécriture en DDD
    - ⇒ suivi de progression: comptage d’évènement générés par version réécrite.
    - ⇒ acceptation du projet de refonte par équipes et CTO
- [réassurance] collaboration inter-équipe et livraison continue. 🤝
-->

## Obtenir **l’accord et le budget**

1. **Mesurer** / estimer couts et risques liés au problème(s)

2. **S'accorder** avec PO/PM sur priorité problème(s)

3. **Proposer** problème(s) et plan aux stakeholders

    - convaincre avec des chiffres (cf mesures)
    - estimer puis comparer le cout: refonte vs status quo

4. **Rassurer** tout au long de refonte/décommissionnement

---

## Avant et pendant **la refonte**

* Mesurer l'impact tout au long de la refonte
    <!-- pour voir la progression, motiver l’équipe et rassurer les stakeholders (notamment pour qu’ils accordent à nouveau du budget pour de prochains chantiers de refonte) -->

* Bosser à plusieurs, pour alignement et apprentissages

* Déployer à chaque (petite) étape, pour rester en contrôle

* Cranter les améliorations, pour pérenniser améliorations
    <!-- ex: activer un flag “strict” dès que possible, pour assurer que le nouveau code soit plus quali que l’ancien -->

---

## 🍱 **À retenir**

* Legacy: atout, couts et risques pour devs ET entreprise

* Réécriture from scratch: rarement une bonne idée

* Conseil: Mesurer → S'accorder → Proposer → Rassurer

* Dé-risquer par PoC, baby steps et déploiment continu
