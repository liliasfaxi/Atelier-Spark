See mkdocs [Cheat Sheet](https://yakworks.github.io/mkdocs-material-components/cheat-sheet/)

italique
_input_

gras
**50070**

image
![Batch Processing](img/batch.png)
ou
<center><img src="../img/tp1/purchases-tail.png"></center>


lien
[Apache Hadoop](http://hadoop.apache.org/)

code
``` Bash
  git clone https://github.com/liliasfaxi/hadoop-cluster-docker
```

inline code
``` hadoop fs -mkdir -p /user/root```

warning
!!! warning "Attention"
    blablabla


error
!!! bug "Erreur"
    blablabla

exercice - activité
!!!question "Activité"

      Modifier

tables
|Instruction|Fonctionnalité|
|---------|-------------------------------------------------------------|
| ```hadoop fs –ls``` | Afficher le contenu du répertoire racine |
| ```hadoop fs –put file.txt``` | Upload un fichier dans hadoop (à partir du répertoire courant linux) |
| ```hadoop fs –get file.txt``` | Download un fichier à partir de hadoop sur votre disque local |
| ```hadoop fs –tail file.txt``` | Lire les dernières lignes du fichier   |
| ```hadoop fs –cat file.txt``` | Affiche tout le contenu du fichier  |
| ```hadoop fs –mv file.txt newfile.txt``` |  Renommer le fichier  |
| ```hadoop fs –rm newfile.txt``` | Supprimer le fichier  |
| ```hadoop fs –mkdir myinput``` | Créer un répertoire |
| ```hadoop fs –cat file.txt \| less``` | Lire le fichier page par page|
