Joris Bouland
Florian Le Brech


Tuto installation du projet ZEND


Fichier pour les Log
L'emplacement d'écriture des logs dépend de la machine. Il faut utiliser un dossier ne nécessitant pas les droits d'administrateur.
Il faut modifier par exemple la ligne 29 dans le fichier zend_tuto\config\autoload\global.php  comme ceci:
$writer = new Zend\Log\Writer\Stream('C:\xampp'. date('Y-m-d') . '-error.log');

Base de données
Vous devez ajouter la base de donnée fournie dans le dossier cache.

Autre
Il peut être nécessaire de cocher la case "Copy files on project open" dans les propriétés du projet.

Tests
Les tests peuvent être effectués avec 2 comptes: admin (mot de passe: admin) et test (mot de passe: test).

