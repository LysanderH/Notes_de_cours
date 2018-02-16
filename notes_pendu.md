# DCS Pendu

## page de départ

* le début constitue correspond à une requête en get
* une constante pour le nombre de mots maxi
* tirer un mot au haard dans une liste de mots
* quelle est la taille de ce mot ?
* créer une chaîne fantôme => décider un caractère de substitution (les ******** remplace sodomie)
* à quel essai (à 9) infructueux est-ce que je me trouve?
* calculer le nombre d'essai restant en soustrayant le nombre d'essai infructueux du nombre d'essai maxi
* besoin d'avoir un alphabet

## Si on joue

* soumettre une lettre en _POST_
* vérifier que la lettre fait partie du mot
	* Si elle est présente
		* remplacer dans la chiane fantôme les cractères de substitution par les lettres trouvées
		* est ce que le mot trouvé correspont à la chine fantome?
			* Si oui, on affiche plus le form
			* On affiche un message de vitoire
	* Si elle n'est pas présente
		* mettre l'image a jour
		* mettre a jours les essais restants
* ajouter la lettre essayée à la liste des lettres essayées
* mettre à jours le select avec les lettres a proposées (car elle disparaissent au fur et a mesure)

## Notes extra

* shaînes de caractères plus grands qu'un octets mb_
* [clef => 'valeurs']