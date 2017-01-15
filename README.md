# elasticsearch-101

**ElasticSearch 101** est un workshop permettant de découvrir la base de données NoSQL ElasticSearch et son écosystème, étape par étape.

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons Licence" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a>

Lors de la mise en oeuvre de ce workshop, n'hésitez pas à vous appuyer sur la [documentation officielle de ElasticSearch](https://www.elastic.co/guide/en/elasticsearch/reference/current/index.html)

## Introduction
**ElasticSearch** est un moteur de recherches orienté documents qui a été créé par Shay Banon. **ElasticSearch** est basé sur la librairie [**Lucene**](http://lucene.apache.org/core/) qui est destinée à l'indexation full-text.

Basé sur le principe d'inverse inversé, **ElasticSearch**  permet d'indexer des documents au format **JSON**. Il se base sur une API RESTful. Il est totalement scalable (contrairement à Lucene) et hautement disponible. Il s'appuie sur un système de réplications et de quorum.

Du point de vue du **CAP**, en cas de partitionnement réseau ou d'indisponibilité de certains noeuds, une majorité de noeuds est nécessaire pour permettre au service d'être disponible, nous perdons la **Disponiblité**.

Les principales fonctionalités d'**ElasticSearch** sont les suivantes :

* Indexation/Recherche **full-text** : *Tous les documents qui contiennent le mot “moteur”*
* Indexation/Recherche **structurée** : *Tous les documents créés entre le 01/10/2014 et le 31/12/2014*
* **Agrégations** : *Répartition des documents, par mois, par type, par ...*
* **Suggestions**
* **Percolateur** : *Quelles sont les requêtes qui correspondent à un document ?*

ElasticSearch dispose en outre d'un des écosystème les plus riches parmi les bases de données NoSQL. La stack Elastic (anciennement **stack ELK**), qui comprend [**Logstash**](https://www.elastic.co/fr/products/logstash), [**Kibana**](https://www.elastic.co/fr/products/kibana) et [**Beats**](https://www.elastic.co/products/beats) est très utilisée pour la centralisation de logs.

## Étapes du workshop

* Étape 0 - [Installation](./instructions/step-0.md)
* Étape 1 - [Opérations CRUD](./instructions/step-1.md)
* Étape 2 - [L'API de recherche](./instructions/step-2.md)

## Liens utiles

* Site officiel : https://www.elastic.co
* La documentation officielle : https://www.elastic.co/guide/en/elasticsearch/reference/current/index.html
