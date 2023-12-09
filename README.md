# Algo-texte

Le but du projet est de pouvoir reconnaitre le genre d'un film à partir de ça description et du nom du film.

## Notebooks

Les notebooks répertorie plusieurs méthodes qui permettent de faire cette analyse, qui sont comparés afin de voir laquelles est la plus efficace.

## TAL

Permet une visualisation des résultats (avec l'utilisation des transformers car la plus précise) via une page web créer localement.

Pour cela:

```shell
cd ~
wget "https://archive.apache.org/dist/lucene/solr/8.3.0/solr-8.3.0.zip"
unzip solr-8.3.0.zip -d
# lien symbolique pour accès facile 
ln -s solr-8.3.0 solr
```
Ensuite

```shell
# depuis la racine de l'outil
./bin/solr start
./bin/solr create -c projet
```

Ensuite il faut remplacer les fichiers qui se trouve dans server/solr/projet par ceux dans TAL/projet du repo

La page web sera visible à l'adresse:
localhost:8983/solr/projet/browse
