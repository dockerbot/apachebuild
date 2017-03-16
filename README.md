# Pour crée une page web avec Docker
---
## Téléchargement

### Télécharge le fichier "apachebuild" avec les trois documents:
 * _apache-config.conf_	
 * _Dockerfile_
 * _instruction&installation.md_

### Pour vérifier le téléchargement, tape:
```
cd apachebuild
ls
```

Tu dois voir le trois documents listé ci-dessus.

---
## Installation

### Crée le directory nommé "www".
```
mkdir www
cd www
```

### Avec "nano", crée un document nommé "index.php".
```
nano index.php
```

Tu vas copier et coller tous ton php code dans ce document.

### Encore, vérifie le contents de "apachebuild".
### Tu dois voir:
 * _apache-config.conf_
 * _Dockerfile_
 * _instruction&installation.md_
 * _**www**_

---
## Lancement

### Construis la page.
```
docker build -t IMAGE\_NOM .
```

### Exécute la page et l'assigne à un port.
```
docker run -d -p NOMBRE\_DU\_PORT:80 IMAGE\_NOM
```

Recherche "localport:NOMBRE\_DU\_PORT" sur un navigateur pour voir la page web.

#### Pour effacer, arrête la container de l'image:
``` 
docker stop CONATINER\_ID
```
---

