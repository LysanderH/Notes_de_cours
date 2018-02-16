# Vocabulaire

* scope/portée: champs dans lequel notre symbol est utilisable/reconnu.
	* il faut travailler dans le plus petit scope possible
	* scope d’une var est la fonction
* let autre possibilité de définir une variable mais autre scope (limité au bloc pas à la var)
* refactoring vise a créer un code réutilisable
* D.R.Y. = Don't Repeat Yourself
* this est l’objet utilisée / this représente l’objet
* évènement = click
* écouteur d’évènement = .AddEventListener/.on
* propagation des évènements ('false' arrète la propagation)
* e.target
* Loi de la proximité qui dit que les éléments proches donnent un ensemble de ces éléments
* Loi de Fiz plus grande zone de click = confort
* système de délégation
* JSon

```
$(document).ready(function() {
  $('button').on('click', function(e) {
    var message = $('<span>Call 1-555-jquery-air to book this tour</span>');
    $('.usa').append(message);
    $(e.target).remove();
  });
});
```

Javascript donne une référence que je peux utiliser ici le paramètre e (qui est égal au click, donc la cible du click)

```
class TodoList{
	$taskList = [];
	function addTask(){

	}
	function deleteTask(){
		$this // fait référence à TodoList mais elle s'évalue ap
	}
}
// C'est le moment ou on utlise la fonction
$list = new TodoList();
$list = new TodoList2();
```
```
for(var i=0, i<docment.querySelector('#list').children.length)
```
Mauvais car a chaque fois les éléments sont conté

[Velocity.js pour animation](http://velocityjs.org/)
