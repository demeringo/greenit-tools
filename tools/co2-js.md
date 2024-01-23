# Co2.js

## Créé par

The Green Web Foundation

## Description

Librairie Javascript open source pour estimer les émissions de GES des applications et sites.

Fonctionne dans le navigateur ou en node.

Il y a des fonctions pour vérifier si un site est hébergé chez un fournisseur qui utilise de l'énergie renouvelable.


## Modèle économique

FOOS

## Modèle de partage

FOOS

## L'outil est-il multicritère ?

Non

## Transparence de l'algo et des données

L'outil est open source.

Les deux modèles 1 byte model du Shift Projet et le Sustainable Web Design Model de la Green Web Foundation sont publiquement décrits.

Il y a une page expliquant la méthodologie : https://developers.thegreenwebfoundation.org/co2js/explainer/methodologies-for-calculating-website-carbon/

La liste des hébergeurs « verts » (qui utilisent des énergies renouvelables) est maintenue par la Green Web Foundation et est open source.

## Quelle base de données, algorithme ou modèle est utilisé ?

Il y a deux modèles possibles : le 1 byte model du Shift Projet et le Sustainable Web Design Model de la Green Web Foundation.
Le second est utilisé par défaut.

Utilise des intensités carbone de l'électricité par pays venant de [Ember](https://ember-climate.org/data/data-tools/data-explorer/) et de [UNFCCC](https://unfccc.int/).

### Sustainable Web Design

La quantité de données transférée est utilisée come proxy pour estimer la quantité d'énergie utilisée.

Les chiffres fournis sont : 
- 15% du total pour l'utilisation des datacenters
- 14% pour l'utilisation du réseau
- 52% pour l'utilisation de l'appareil
- 19% pour la fabrication de tous ces appareils

L'énergie est ensuite convertie en émissions de GES avec les bases Ember et UNFCCC.

### One Byte Model

Le One Byte Model utilise aussi la quantité de données transférée comme base.

Dans CO2.js, seules le serveur et le réseau sont estimés.

## Qualités et avantages

- Simple à utiliser
- Peut-être inclus dans des programmes Javascript, ce qui est pratique
- Open source et bien documenté, y compris au niveau méthodologique

## Inconvénients et limites

- Monocritère
- Ne peut faire que des estimations
- Se base uniquement sur les données réseaux, ce qui est un proxy très partiel
- Biais de linéarité

## Commentaires



