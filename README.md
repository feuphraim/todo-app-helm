# Todo App - Chart Helm Kubernetes

Ceci est un chart Helm pour déployer une application Todo sur Kubernetes. Conçue initialement pour démontrer l'architecture conteneurisée, cette chart facilite le déploiement pour illustrer les principes de configuration et de déploiement via Helm, avec: 
- Intégration base de données MySQL
- Stockage sur volume persistant
- Support Nginx Ingress
- Options de service et déploiement configurables


---

## 🛠 Prérequis

- Cluster Kubernetes (1.19+)
- Helm (v3)
- Contrôleur Ingress Nginx
- kubectl

## 🔧 Paramètres de Configuration

| Paramètre | Description | Défaut |
|-----------|-------------|---------|
| `replicaCount` | Nombre de réplicas de l'application | `1` |
| `image.repository` | Dépôt d'image Docker | `getting-started-app` |
| `image.tag` | Tag de l'image Docker | `v2` |
| `mysql.host` | Hôte du service MySQL | `mysql.default.svc.cluster.local` |
| `persistence.size` | Taille du volume persistant | `10Gi` |

## 🔒 Considérations de Sécurité

- Personnaliser les identifiants MySQL
- Utiliser les Secrets Kubernetes pour les données sensibles
- Envisager l'utilisation de politiques réseau

## 🤝 Contribution

1. Forker le dépôt
2. Créer une branche de fonctionnalité
3. Commiter vos modifications
4. Pousser la branche
5. Ouvrir une Pull Request

## 📄 Licence

Distribué sous la Licence MIT.

## 🚦 Statut

v1 terminé

---

Si vous avez besoin de clarifications ou d'exemples de configuration, dites-le-moi ! 😊
