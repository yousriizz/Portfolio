---
title: Mise en place du HSRP
publishDate: 2024-12-01 00:00:00
img: /assets/stock-3.jpg
img_alt: Pearls of silky soft white cotton, bubble up under vibrant lighting
description: |
  Nous avons mis en place HSRP sur des routeurs pour une redondance optimale.
tags:
  - Cisco Packet Tracer
  - Prise en main de routeur
  - PuTTy
---

> Documentation du Projet : Mise en Place de HSRP sur des Routeurs

### Introduction

Le protocole HSRP (Hot Standby Router Protocol) est une solution de redondance permettant d'assurer une disponibilité élevée dans un réseau en désignant un routeur actif et un routeur en veille. Ce projet vise à configurer HSRP sur un ensemble de routeurs pour garantir une continuité de service en cas de défaillance d'un routeur principal.

### Objectifs du Projet

- Fournir une redondance de passerelle par défaut : Les hôtes du réseau doivent toujours disposer d'une passerelle opérationnelle, même en cas de panne.
- Minimiser le temps d'indisponibilité : Permettre un basculement transparent entre les routeurs actif et de secours.
- Assurer une configuration robuste et évolutive : La solution doit être simple à maintenir et adaptable à l'échelle du réseau.

### Matériel et Logiciels Utilisés

- Routeurs Cisco
- Logiciel de gestion : CLI (Command Line Interface) via PuTTY
- Topologie : Deux routeurs connectés à un réseau LAN commun

> Avantages de HSRP 

- Redondance : HSRP garan3t une disponibilité constante de la passerelle pour les
u3lisateurs. Si un routeur devient indisponible, un autre routeur prend
automatiquement le relais.

- Simplicité : Sa configura3on est relativement simple et ne nécessite pas de matériel
spécialisé.

- Transparence : Les utilisateurs finaux ne remarquent pas les basculements, car tout
se fait de manière transparente.

- Haute disponibilité : C’est un élément clé dans les réseaux critiques nécessitant une
fiabilité élevée.

> Inconvénients de HSRP

- Consomma3on de ressources : Tous les routeurs HSRP doivent rester actifs, bien
que seul le routeur principal gère activement le trafic, ce qui peut être un gaspillage
de ressources.
- Basculement retardé : Bien que rapide, le temps de basculement peut ne pas
convenir aux applications nécessitant une latence extrêmement faible.
- Dépendance au matériel : En cas de panne matérielle majeure sur tous les routeurs
du groupe, HSRP ne pourra pas garantir la redondance.
