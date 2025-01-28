# Modèles de ressources

Un modèle de ressource est contitué de propriétés provenant d'un ou plusieurs [vocabulaires](vocabulaires.md).

Le modèle de ressource est le premier élément sélectionnable lors de la [création/édition d'une ressource](ressources.md#formulaire-de-créationédition) dans l'onglet **Avancée**.
Il permet de prédéfinir un liste de champs pour décrire les ressources et peut également servir de filtre lors des recherches.

## Créer un modèle

![Création d'un modèle de ressource](assets/creation-modele.png)

Dans le menu **Modèles de ressource** (1), le formulaire de création d’un modèle
est accessible avec le bouton **Ajouter un nouveau modèle** (2).

![Formulaire de création d'un modèle de ressource](assets/formulaire-modele.png)

Un libellé est obligatoire (3).

La liste des propriétés est affichée à droite sous forme de menus dépliables par
vocabulaire (4).

Il est possible de chercher une propriété en saisissant le nom de la propriété
dans la zone de saisie. La recherche se fait dans la langue de l'administration.

Les propriétés du modèle apparaîtront à la suite du formulaire (5).

Pour chaque propriété (6), il est possible :

* d’accéder aux informations de celle-ci (icône 3 points)
* de paramétrer la propriété uniquement dans ce modèle de ressource (icône stylo)
* de la retirer du modèle de ressource (icône poubelle)

En cliquant sur l'icône stylo d'une propriété, un menu sur la droite s'ouvre.

![Paramètre d'une propriété dans un modèle de ressource](assets/parametre-propriete-modele.png)

Le titre alternatif (7) permet de modifier le nom de la propriété à l'affichage.

L'utilisation d'un libellé aternatif ne change l'affichage que lorsque le modèle est utilisé. Les paramétrages dans Omeka S, par exemple de l'instance Omeka S ou d'un site, n'en tiendront pas compte.

---

Le commentaire est affiché dans les formulaires de création/édition des ressources pour chaque propriété. Il permet de donner des indications sur la manière de les remplir (une norme à respecter, une manière d'écrire une valeur, etc.).

Le commentaire alternatif (8) permet de remplacer le commentaire d'origine uniquement dans ce modèle de ressource.

---

Le paramètre **Requis** (9) permet d'imposer d'avoir une valeur dans la propriété.

---

Le paramètre **Privé** (10) masquera la propriété lors de l'affichage des sites publics. Les valeurs renseignés dans ces champs seront automatiquement misent en privé lors de la création d'une ressource.

---

Le paramètre **Types de données** (11) permettent de sélectionner les types de valeurs qui peuvent être renseignés dans la propriété (par défaut : texte, uri et ressource) dans les formulaires de création/édition d'une ressource.

Plusieurs modules permettent d'ajouter des types pour avoir des vocabulaires personnalisés gérés dans Omeka S (Custom Vocab), l'utilisation de thésaurus (Value Suggest) ou l'éditorialisation en HTML (Data Type RDF)

---

**Ne pas oublier d’appliquer les modifications lors du paramétrage de chaque propriété (12).**

## Éditer un modèle

![Édition d'un modèle de ressource](assets/edition-modele.png)

Dans le menu **Modèles de ressource** (1), le formulaire d’édition d’un modèle est
accessible avec l'icône stylo (2).

La page d’édition est la même que celle de [création](modeles-ressource.md#créer-un-modèle).

La modification du paramétrage d'une propriété d'un modèle ne va pas mettrent les valeurs des ressources utilisant ce modèle à jour. Cela nécessite des opérations supplémentaires.

## Types de données

Omeka S propose par défaut les types de données texte, URI et ressource pour mettre par exemple des contenus en relations entre eux.

Des modules peuvent être ajoutés pour proposer plus de types de données pour configurer les modèles de ressources

### Data Type RDF

Ce module permet d'ajouter les types données suivants :

- HTML (avec un éditeur similaire à celui des pages)
- XML
- Booléen
- JSON

[https://omeka.org/s/modules/DataTypeRdf/](https://omeka.org/s/modules/DataTypeRdf/)

### Numeric Data Type

Ce module permet d'ajouter les types de données suivants :

- Date
- Entier
- Durée
- Intervalle de date

[https://omeka.org/s/modules/NumericDataTypes/](https://omeka.org/s/modules/NumericDataTypes/)

### Value Suggest

Ce module permet d'ajouter pour une propriété l'interrogation des thésauri, des référentiels ou des vocabulaires de manière dynamique depuis les formulaires d'édition de ressources comme Geonames, IdRef, OpenTheso (par exemple Pactols).

La liste des référentiels intérrogeables est disponibles sur la page de présentation du module sur le site d'Omeka :

[https://omeka.org/s/modules/ValueSuggest/](https://omeka.org/s/modules/ValueSuggest/)

### Custom Vocab

Ce module permet d'ajouter des listes controlées de valeurs qui sont gérées dans l'instance Omeka S.

Le menu pour créer des [vocabulaires personnalisés](module-custom-vocab.md) est disponibles dans le menu de gauche dans l'administration.

[https://omeka.org/s/modules/CustomVocab/](https://omeka.org/s/modules/CustomVocab/)