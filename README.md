# Popeye project

Popeye est est un projet sur la conteneurisation d'une application web. Il s'agit d'une application de vote en temps réel. L'application est composée de 5 services :

- **DB** : Service de base de données
- **Pool**-UI : Service de l'interface utilisateur
- **Result** : Service de résultat
- **Worker** : Service de travailleur
- **Redis** : Service de cache

## Features

### Obligation

Stack MERN ( MongoDB, Express, React, NodeJS)

### Ports utilisés

- **Redis** : 6379
- **DB** : /
- **Pool** : 5000
- **Result** : 5001
- **Worker** : /

## Get started

### Prerequisites

- Docker (https://docs.docker.com/get-docker/)

### Installation

```
git clone git@github.com:EpitechMscProPromo2026/T-DOP-601-NAN_alexandre-tressel.git
cd T-DOP-601-NAN_alexandre-tressel
docker compose up --build -d
-> http://localhost:5000 (Pool)
-> http://localhost:5001 (Result)
```

## Screenshot
