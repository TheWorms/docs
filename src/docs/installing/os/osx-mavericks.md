# OS X Mavericks

## Logiciels requis

Tout d'abord, installez les programmes suivants:


-   <http://nodejs.org/>
-   <http://brew.sh/>

## Installation de NodeBB

Installez redis avec homebrew:

```
brew install redis
```

Démarrer le serveur redis, dans votre terminal, entrez:

```
redis-server
```

Cloner le repo NodeBB:

```
git clone -b v1.10.x https://github.com/NodeBB/NodeBB.git
```

Entrez le répertoire:

```
cd NodeBB
```

Lancer la configuration:

```
./nodebb setup
```

Vous pouvez laisser toutes les options par défaut, sauf "Quelle base de données utiliser?"
use (mongo) ", auquel vous devez répondre" redis "

Et tu as fini! Après l'installation, lancez

```
./nodebb start
```

Vous pouvez acceder à votre forum sur `http://localhost:4567/`
