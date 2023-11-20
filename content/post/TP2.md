+++
author = "Rémi Lacombe"
title = "TP2"
date = "2019-03-09"
description = "Sections fabrication et inventaire"

+++

Sections fabrication et inventaire.
<!--more-->

## 1. Introduction

Cela fais quelques mois que ma boutique en ligne fonctionne, j'ai vendu des milliers de canards et le temps devient un peu long. Il est temps de commencer un nouveau projet : **l'internalisation de la fabrication de canards en plastique !**  
**C'est parti !**

L'un de mes gros clients à une forte de demande en canard de couleur verte, ce sera donc le premier produit que je fabriquerai !  
J'établi pour cela une nomenclature des opérations :  

{{< diag >}}

## 2. Activité demandée

### 2.1. Création des postes de charges

Comme montré plus haut, j'ai identifié deux postes de charge. Je dois maintenant les créer dans mon ERP :

![Poste de moulage](/PosteDeTravail.gif)

On fait de même pour le poste de peinture.

### 2.2. Création des gammes

On créera les opérations dans la partie 2.4.

### 2.3. Création des articles

Je crée les matières premières (A1,A2,A3 et A4), le sous-produit en sortie de moulage(SP1) ainsi que le produit fini (PF).

![Produits fabrication](/ProduitsFabrication.gif)

### 2.4. Créations des nomenclatures

Les produits créés, il faut à présent indiquer les nomenclatures :
On commence par la nomenclature du produit **"Canard sortie de moulage"**.  
On indique qu'il faut 0.2 unités de granule de caoutchouc. On spécifie également l'opération **"Moulage"** en précisant le poste de charge **"Station de moulage"**

![Nomenclature moulage](/NomMoulage.gif)

De même pour le produit fini **"Canard Vert"**. On saisi la nomenclature en ajoutant le produit **"Canard sortie de moulage"** ainsi que tout les types de peinture et leurs quantités respectives. On crée une opération **"Peinture"** dans le poste de charge **"Station de peinture"**

![Nomenclature peinture](/NomPeinture.gif)

### 2.5. Rapports Structure nomenclature et coût

J'effectue quelques modifications dans les capacités et coûts des postes de travail pour avoir des résultats plus cohérents.  
Un exemple de changement effectué est la fabrication de plusieurs canards en même temps, cela permet de n'avoir qu'un seul temps de réglage et de nettoyage pour un lot. On fera ici des lots de 50.
Après modification, voici le rapport de nomenclature du produit **"Canard Vert"**.

{{< pdf_viewer file="Odoo Report BOM" >}}

### 2.6. Faire deux commandes clients avec des variantes couleurs différentes

Un client me réclame des canards rouges !
On renomme le produit **"Canard Vert"** en **"Canard Uni"** et on y ajoute deux variantes.

![Variantes](/Variantes.gif)

On crée un nouveau produit pour la peinture rouge. Il faut également ajouter une nomenclature pour la variante rouge. Voici les 3 nomenclatures ainsi créées.

![NewNom](/NewNom.gif)

Une fois que cela est fait, on peut enfin rentrer les commandes :

StarkIndustries commandent 50 canards verts :

![Order Vert](/OrderVert.gif)

Et Monster .inc commandent 100 canards rouge :

![Order Rouge](/OrderRouge.gif)

### 2.7. Lancer un ordre de fabrication
