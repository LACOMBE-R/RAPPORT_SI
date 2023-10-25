+++
author = "Rémi Lacombe"
title = "TP1"
date = "2019-03-09"
description = "Sections achat et vente"

+++

## Lien du serveur Odoo

[Site](https://tp_odoo.rioc.fr)

Login : <IRPAUC05@example.com>  
mdp : I4PAUC05

## Introduction

<!-- A modifier -->
Ce matin, au réveil, une idée **incroyable** m'est venue, je vais tout plaquer et vendre des **canards en plastique** sur internet !  
Bien sûr...pour passer de l'idée, il me faut un bon outil de gestion.  
J'ai choisi Odoo car Open-Source et facile d'utilisation !
L'objectif de cette première partie est d'établir un processus d'achat vente.
**C'est parti !**

## 1. Création des données de base

### 1.1. Créer un entrepôt et un emplacement

Pour vendre mes canards, j'ai acheté un **entrepôt**, je dois maintenant l'ajouter à mon nouvel **ERP** !

Aprés s'être rendu sur le panneau **inventaire**, on crée un entrepôt:  
![Création d'un entrepot](/Entrepot.gif)

Pour m'y retrouver un peu mieux au milieu de tout ces canards, je crée un emplacement:  
![Création d'un emplacement](/Emplacement.gif)

### 1.2. Créer deux clients

Il faut maintenant créer des clients qui achèteront nos canards en plastique !

Pour cela, rendez vous dans le panneau **vente**:  
![Création d'un client](/Client.gif)

On fera de même pour mon second plus gros client, **Monsters Inc**;

![Création d'un deuxième client](/MonstersInc.png)

### 1.3. Créer un fournisseur

Pour vendre mes canards, je dois d'abord les acheter chez un fabricant.  
L'entreprise DuckMaker offre une gamme diversifiée de canards en tous genres, ça sera parfait !  
On renseigne le fournisseur dans le panneau **Achats**:

![Création d'un fournisseur](/Fournisseur.gif)

### 1.4. Créer un produit

On peut finalement créer notre premier produit !  
Après une rapide étude de marché (et parce que c'est classe) mon premier produit sera un **canard robot** !

![Création d'un fournisseur](/Produit.gif)

## 2. Processus d'achat vente

## 2.1. Création de devis

Maintenant que ma boutique est en ligne, mes première commande me sont parvenues.
Je dois maintenant créer des devis. D'abord pour Stark Industries:

![Création du devis 1](/Devis1.gif)

Puis pour Monster, Inc:

![Création du devis 2](/Devis2.gif)

Pour transmettre ces devis aux clients je peux les imprimer ou les exporter:

{{< Odoo_Report >}}

Si ce devis est validé par le client, je peux en faire un bon de commande:

![Bon de commande](/DevisToBonDeCommande.gif)

Une nouvelle ligne apparaît dans le tableau de commande avec la mention "à facturer":  
***(Suite à une petite erreur, le numéro de commande à changé, mais rien de grave !)***

![Création de facture](/Facturation.gif)
