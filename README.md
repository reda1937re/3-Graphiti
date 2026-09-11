# 3-Graphiti

Deux scripts CLI implémentant un modèle de données en graphe pour un "Personal Fitness Tracker" (pas un chatbot). `grahp_caracts_custumers.py` se connecte à une vraie base Neo4j pour stocker des activités sportives comme nœuds de graphe et exécuter des requêtes Cypher (activités récentes, filtres par distance/type). `demo_offline.py` simule les mêmes opérations en mémoire, sans connexion base de données requise.

## Tech stack

neo4j (AsyncGraphDatabase driver), asyncio, python-dotenv

## Lancer le projet

```bash
pip install neo4j python-dotenv
python demo_offline.py          # sans base de données
python grahp_caracts_custumers.py  # nécessite une instance Neo4j + .env (NEO4J_URI, NEO4J_USER, NEO4J_PASSWORD)
```
