
![Scale up](Scale-up.png)

### **Explication des éléments supplémentaires**

**Infrastructure Web Standard** Dans une infrastructure web typique, les **serveurs web** et **serveurs applicatifs** ont des rôles distincts :

-   **Serveur Web** : Traite les requêtes HTTP, sert du contenu statique (HTML, CSS, JS) et transmet les requêtes dynamiques au serveur applicatif (exemples : **Nginx**, **Apache**).
-   **Serveur Applicatif** : Exécute la logique métier, traite le contenu dynamique et interagit avec la base de données (exemples : **Node.js**, **Tomcat**, **Django**).

### **Configuration de l’infrastructure**

Pour construire une infrastructure **scalable** et **résiliente**, les composants suivants sont nécessaires :

**Serveur**

-   Agit comme **serveur web**, gérant les requêtes HTTP/HTTPS.
-   Sert les fichiers statiques et redirige les requêtes dynamiques vers le serveur applicatif.

**Load Balancer (HAProxy)**

-   Répartit le trafic entre plusieurs serveurs pour assurer **la haute disponibilité et la scalabilité**.
-   Configuré en **cluster** avec un second load balancer pour garantir la redondance.

**Séparation des composants**

-   **Serveur Web** : Dédié aux requêtes HTTP/HTTPS et à la gestion des fichiers statiques.
-   **Serveur Applicatif** : Traite la logique métier et génère le contenu dynamique.
-   **Base de données** : Gère le stockage et la gestion des données.

### **Explication des choix d’architecture**

**Pourquoi ajouter un Load Balancer (HAProxy) ?**

-   **Objectif** : Répartir le trafic de manière équilibrée pour éviter la surcharge d’un serveur unique.
-   **Bénéfices** : Améliore **la disponibilité**, **la scalabilité** et **la tolérance aux pannes**.
-   **Configuration en cluster** : En cas de défaillance d’un load balancer, un autre prend le relais.

**Pourquoi séparer les composants (serveur web, serveur applicatif, base de données) ?**

-   **Serveur Web** : Gère exclusivement les requêtes HTTP/HTTPS et le contenu statique. Cette séparation optimise l’utilisation des ressources.
-   **Serveur Applicatif** : Exécute la logique métier et génère du contenu dynamique, améliorant la performance et l’évolutivité.
-   **Base de données** : Dédiée au stockage et à la gestion des données pour garantir l’intégrité et la sécurité des informations.