1 - Quelles options semblent spécifiques à Docker Swarm ?
    healcheck, depends_on, deploy et replicas

2 - Dessiner le schéma d'architecture associé au fichier docker-stack.yml => Voir Services & Réseaux.png

3 - Que signifie la ligne Processed by container ID […] ?
    Affiche l'ID du conteneur docker

4 - Pourquoi varie-t-elle ? L'id ne doit surement pas être fixe et en cas de modification il doit en générer un nouveau

5 - Play with Docker : Lesquelles et pourquoi ?
    Hostname, 2ème et 3ème IP, RemoteAddr, Cookie (Voir Play with Docker.png)

6 - Que fait mode: global ? D'après la doc, pour le mode replicated on doit spécifier le nombre de tache et le swarm manager va les répartir sur les noeuds disponible alors qu'avec le mode global le manager va placer une tache sur chaque noeud disponible

7 - Commande pour déchoir et promouvoir un noeud : 
    docker node promote 
    docker node demote

8 - Notion d'équivalence entre Kubernetes et Swarm
    Deploy : replicas => spec : replicas
    image => spec : container : image
    ports => ports & targetPort