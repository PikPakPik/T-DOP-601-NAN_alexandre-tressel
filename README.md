# Popeye project

Popeye est est un projet sur la conteneurisation d'une application web. Il s'agit d'une application de vote en temps réel. L'application est composée de 5 services :

- **Front en Python (Poll)** : Une page web où les gens votent. Utilise Flask pour collecter et envoyer les votes à Redis.

- **Result en Node.js** : Une page web qui montre les résultats des votes. Utilise Node.js avec Socket.io pour aller dans la base de données PostgreSQL et récupérer les votes en temps réel.

- **Worker en Java** : Un programme qui prend les votes de Redis, les traite, et les enregistre dans une base de données PostgreSQL.

- **DB avec PostgreSQL** : Une base de données qui garde les votes de manière sûre et permet de les récupérer facilement.

- **Redis** : Un système rapide pour stocker temporairement les votes entre le moment où ils sont faits et le moment où ils sont traités.

[![](https://mermaid.ink/img/pako:eNpFzj0KwzAMBeCrBM3xBdwt-AAlLXTxImKlMfFPkO2hhNy9CoRWk_jeA2mHKTsCDW_Gbeme5mZTJ3PPOSilRnK-XDRSaaEKmuEnkgq8Mq_EF5rhL9BDJI7onVzYz9xCXSiSBS2rQ14t2HRID1vNj0-aQFdu1EPbHFYyHuWxCHrGUOj4AgFWNt8?type=png)](https://mermaid.live/edit#pako:eNpFzj0KwzAMBeCrBM3xBdwt-AAlLXTxImKlMfFPkO2hhNy9CoRWk_jeA2mHKTsCDW_Gbeme5mZTJ3PPOSilRnK-XDRSaaEKmuEnkgq8Mq_EF5rhL9BDJI7onVzYz9xCXSiSBS2rQ14t2HRID1vNj0-aQFdu1EPbHFYyHuWxCHrGUOj4AgFWNt8)

## Features

### Obligation

Application de vote en temps réel fournie dans le module

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
docker compose up --build
-> http://localhost:5000 (Pool)
-> http://localhost:5001 (Result)
```

## Screenshot

![7DpxzEFVyo67ZiYtmKYc2Bx6xcYskko3CnHW9jtH](https://github.com/EpitechMscProPromo2026/T-DOP-601-NAN_alexandre-tressel/assets/57991630/4bd61c6c-2438-44f4-af22-02a341c47699)
