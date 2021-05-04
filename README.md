# mysql-8gb-config

## C'est quoi ?
Un exemple de configuration pour un serveur PHP7.3 + MySQL ayant 8gb de RAM à se répartir pour faire tourner des sites exécutant beaucoup de requêtes SQL assez lourdes. 

Attention cependant, car si vous faites tourner d'autres paquets tels qu'un serveur mail, il est possible que vous atteignez la limite de RAM de votre serveur.

Liste des configurations MySQL : 
- 8gb : https://github.com/thomas-ddev/mysql-8gb-config
- 16gb : https://github.com/thomas-ddev/mysql-16gb-config


## Est-ce qu'il faut configurer autre chose ?
Oui, il faut penser à augmenter la limite de la variable "open_files" à 65535 sous peine de brider les performances de MySQL. Vous pouvez obtenir cette limite via la commande : `ulimit -n`
