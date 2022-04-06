# brief_docker
Nous avons ouvert un Ubuntu
Créer un dossier `mkdir docker-covid-Brief`
Puis sommes rentré dans le dossier: `cd docker-covid-Brief`
Et enfin nous avons ouvert VS Code avec `code .`

Nous avons créé 4 fichier:

 - fichier python `main.py` -> ouvrir la connection avec MySQL
 - fichier `Dockerfile` -> paramètrer le code
 - fichier `docker-compose.yml` -> Créer les containers dans Docker et fait le lien entre la bdd et grafana
 - fichier `devcontainer.json` -> Echange de données

Les trois derniers fichiers ce trouve dans un dossier `.devcontainer`

Après cela nous téléchargeons sur VS Code l'extension `VS Code Remote-Containers extension`
Il permet de créer les containers dans Docker.
Nous allons par la suite chercher cette extension dans une ` Command Palette`
Et ouvrir `Remote-Containers: Open Folder in Container ...`
Cela nous envoi nos dossier dans un Workspace du nom de `Dev Container: Develop Python`

Nous ouvrons MySQL avec un `localhost:8080` et nous connectons avec les données fournies dans `main.py`
On import le fichier `vaccination.sql`
Après cela nous pouvons ouvrir Grafana grâce au lien `localhost:3000`
Nous nous connectons, faisons le lien avec la bdd depuis `DATA Sources`

Pour finir nous avons fait deux graphiques avec le dashboard.

Voici les graphiques avec leur requêtes:

![graph](/totalvaccs.png)

![graph](/vaccination_journalier.jpg)
