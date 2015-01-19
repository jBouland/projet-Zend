Joris Bouland
Florian Le Brech


Tuto installation du projet ZEND

//**** SI VOUS AVEZ DÉJA RECUPERER LE PROJET ****///
 En principe, un simple "pull" sur le projet devrait marcher.
Vérifier quand même que le projet s'appelle bien "bouland" et non pas "zend_tuto". Si c'est le cas, renommez-le.

//**** SI CEST LA PREMIERE FOIS ****////

Renommez-le projet en "bouland".

Fichier local.php:
Par défaut ce fichier est exclu par git. Pour faire fonctionner la base de données, vous devez ajouter:
 return array(
     'db' => array(
         'username' => 'root',
         'password' => '',
     ),
 );
Prenez à ajouter votre propre mot de passe (et username si nécessaire) pour accéder à votre base de données.

Fichier pour les Log :
L'emplacement d'écriture des logs dépend de la machine. Il faut utiliser un dossier ne nécessitant pas les droits d'administrateur.
Il faut modifier par exemple la ligne 29 dans le fichier bouland\config\autoload\global.php  comme ceci:
$writer = new Zend\Log\Writer\Stream('C:\xampp'. date('Y-m-d') . '-error.log');

Base de données :
Vous devez ajouter la base de donnée fournie dans le dossier cache intitulé "boulandlebrech.sql".

Autre :
Il peut être nécessaire de cocher la case "Copy files on project open" dans les propriétés du projet.

Tests :
Les tests peuvent être effectués avec 2 comptes: admin (mot de passe: admin) et test (mot de passe: test).

