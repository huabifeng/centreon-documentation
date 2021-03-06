---
id: centreon-commercial-extensions
title: Extensions Commerciales
---

## Introduction

Vous trouverez dans ce chapitre tout ce qui concerne les **extensions
commerciales** de Centreon.

> Il est important de mettre à jour en utilisant la documentation adéquate de
> mise à jour et de lire attentivement les notes de mise à jour afin d'être au
> courant de changements qui pourraient impacter votre usage ou votre plateforme
> ou des développements spécifiques que vous auriez fait.

Pour faire des demandes d'évolutions ou reporter des bugs sur les extensions
commerciales, veuillez contacter le support.

## Centreon MAP release notes

### 20.10.1

* Sauvegarder une Geo View sur un Widget Custom View MAP était impossible dû à l'absence du bouton "Sauvegarder"
* Partager les métriques de statistiques d'usage entre le serveur MAP et le Central en HTTPS échouait
* Créer des liens en utilisant l'API REST peut maintenant recourir aux propriétés 'bendpoints', 'displayValue' et 'displayPercent'
* Ajouter des ressources Centreon lors de la création d'un Widget Output par l'API REST est maintenant possible
* Installer MAP Studio lors d'une nouvelle installation échouait à cause de la configuration du back-up automatique

### 20.10.0

#### Enhancements

-   La licence est maintenant entièrement géré sur le serveur Centreon
    Central.

#### Serveur plus rapide pour les cartes complexes

Cette version pose les bases de l'évolution de l'expérience
dans la création et la visualisation de cartes.

La première étape étant la naissance d'un nouveau serveur Centreon MAP
(nom de code **"NG"** pour "Nouvelle Génération"), qui a été conçu pour
être plus puissant, plus rapide et plus léger.

Le serveur est en **phase expérimentale** et est sujet à évolution.

Il n'est utilisé pour le moment que pour la visualisation des cartes. La
création et l'édition de cartes utilisent toujours le serveur que nous
connaissons.

Du côté de l'interface Centreon, tout a été fait pour pouvoir utiliser
ces deux serveurs. Il est ainsi possible de basculer la consultation
des cartes d'un serveur à l'autre facilement.

Pour l'utiliser, il est nécessaire de l'installer et l'activer.
Référez-vous à la [documentation dédiée](../graph-views/install.html#centreon-map-ng)

## Centreon BAM release notes

### 20.10.0

- [Configuration] Mise à jour du style des pages *Activités métiers*
  et *Vues métiers*

## Centreon MBI release notes

### 20.10.0

- Compatibilité avec Centreon 20.10

## Centreon Auto Discovery release notes

### 20.10.2

#### Bugfixes

- [Host Discovery] Des valeurs longues dans le champs *host.ip* provoquent
  l'erreur "Error when sorting and filtering host modification results"
- [Host Discovery] Le script de sauvegarde fonctionne maintenant sous
  CentOS 8

#### Enhancements

- [Host Discovery] Ajout d'une boite de dialogue de confirmation lors de
  la suppression d'une tâche
- [Host Discovery] Changement de la formulation "Paramètres additionnels"
  en "Paramètres de découverte" dans les écrans

### 20.10.1

#### Bugfixes

- Les scripts de mise à jour en doubles dans la version précédente
  entraînent une erreur SQL dans le log

### 20.10.0

> Référez vous à la [Configuration du module Gorgone](../monitoring/discovery/administration.html#configuration-du-module-Gorgone)
> pour vous assurer que la configuration correspond aux prérequis minimaux.

> Si une découverte est effectuée sur un Remote Server ou un Poller,
> assurez-vous que le serveur utilise les derniers composants 20.10.

> Sur un Remote Server, le module Autodiscovery peut être désinstallé depuis
> le menu `Administration > Extensions > Gestionnaire` afin de ne
> pas générer d'erreurs inutiles dans les logs de Gorgone.

#### Host Discovery

L'assistant de découverte d'hôte permet désormais de planifier vos découvertes
de plusieurs manières : annuelle, mensuelle, quotidienne et même
toutes les x heures ou minutes.

Les tâches de découverte planifiées peuvent être suspendues et reprises à
tout moment.

Le résultat de la découverte peut également être traité automatiquement pour
ajouter, désactiver et, si nécessaire, réactiver les hôtes dans la
configuration.

Si vous décidez d'ajouter manuellement les hôtes à partir de la page de
résultats de la tâche, la règle d'association peut maintenant être
modifiée et enregistrée à partir de cette page pour répondre à vos besoins
en appliquant la règle directement sur le résultat.

Les nouveaux modificateurs *d'exclusion* et *d'inclusion* vous aideront à
décider quels hôtes sont censés être ajoutés dans la configuration, et ceux
qui doivent être désactivés ou activés.

Jetez un oeil à cet exemple pour bien comprendre leurs impacts:
[Mettre à jour votre configuration dynamiquement](../monitoring/discovery/hosts-discovery.html#mettre-a-jour-votre-configuration-dynamiquement)

#### Service Discovery

La découverte de service utilise maintenant Gorgone pour exécuter les plugins
de découverte, et par conséquent le système de communication de Gorgone et
non plus des connexions SSH autonomes.

#### Bugfixes

- Contient tous les correctifs jusqu'à la version 20.04.6

## Centreon Plugin Packs Manager release notes

### 20.10.0

- Compatibilité avec Centreon 20.10

## Centreon License Manager release notes

### 20.10.1

#### Bug fixes

- After adding a license or a token the user must access to associated functionalities
- Rights issues with the gnupg library with multiple users (only with Docker)
- Disable 'Add' button when input is empty

### 20.10.0

- Compatibilité avec Centreon 20.10

## Centreon Anomaly Detection

### 20.10.0

- Compatibilité avec Centreon 20.10
