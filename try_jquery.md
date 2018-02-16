# Try jQuery
**3.4**
```var message = $('<span>Call 1-555-jquery-air to book this tour</span>');
$('.book').before(message);
```
**3.5**
```
var message = $('<span>Call 1-555-jquery-air to book this tour</span>');
$('.usa').append(message);
```
**3.6**
```
var message = $('<span>Call 1-555-jquery-air to book this tour</span>');
$('.usa').append(message);
$('.book').remove();
```
**3.7**
```
$('button').on('click', function(){
var message = $('<span>Call 1-555-jquery-air to book this tour</span>');
$('.usa').append(message);
$('button').remove();
});
```
**3.8**
```
$('button').on('click', function() {
  var message = $('<span>Call 1-555-jquery-air to book this tour</span>');
  $('.usa').append(message);
  $('button').remove();
});
```
**3.9**
```
$('.tour').on('click', function() {
  var message = $('<span>Call 1-555-jquery-air to book this tour</span>');
  $('.usa').append(message);
  $('button').remove();
});
```
**3.10**
```
$(document).ready(function(){
  $('button').on('click', function() {
  var message = $('<span>Call 1-555-jquery-air to book this tour</span>');
  $('.usa').append(message);
  $('button').remove();
});
});
```
**3.11**

Vidéo

**3.12**
```
$(document).ready(function() {
  $('button').on('click', function() {
    var message = $('<span>Call 1-555-jquery-air to book this tour</span>');
    $('.usa').append(message);
    $(this).remove();
  });
});
```
**3.13**
```
$(document).ready(function() {
  $('button').on('click', function() {
    var message = $('<span>Call 1-555-jquery-air to book this tour</span>');
    $(this).after(message);
    $(this).remove();
  });
});
```
**3.14**
```
$(document).ready(function() {
  $('button').on('click', function() {
    var message = $('<span>Call 1-555-jquery-air to book this tour</span>');
    $(this).closest('.tour').append(message);
    $(this).remove();
  });
});
```
**3.15**
```
$(document).ready(function() {
  $('.tour').on('click', function() {
    var message = $('<span>Call 1-555-jquery-air to book this tour</span>');
    $(this).append(message);
    $(this).find('button').remove();
  });
});
```

**3.16**

Vidéo

**3.17**

```
$(document).ready(function() {
  $('button').on('click', function() {
    var message = $('<span>Call 1-555-jquery-air to book this tour</span>');
    // create discount variable here
    var discount = $(this).closest('.tour').data('discount');
    $(this).closest('.tour').append(message);
    $(this).remove();
  });
});
```

**3.18**

```
$(document).ready(function() {
  $('button').on('click', function() {
    var discount = $(this).closest('.tour').data('discount');
    var message = $('Call 1-555-jquery-air for a $' + discount + 'discount');
    $(this).closest('.tour').append(message);
    $(this).remove();
  });
});
```

**3.19**

```
$(document).ready(function() {
  $('button').on('click', function() {
    var tour = $(this).closest('.tour');
    var discount = tour.data('discount');
    var message = $('<span>Call 1-555-jquery-air for a $' + discount + ' discount.</span>');
    tour.append(message);
    $(this).remove();
  });
});
```

**3.20**

```
$(document).ready(function() {
  $('.tour').on('click', 'button', function() {
    var tour = $(this).closest('.tour');
    var discount = tour.data('discount');
    var message = $('<span>Call 1-555-jquery-air for a $' + discount + ' discount.</span>');
    tour.append(message);
    $(this).remove();
  });
});
```

**3.21**

```
$(document).ready(function() {
  //Create the click handler here
  $('#filters').on('click', '.on-sale', function(){
  });
});
```

**3.22**

```
$(document).ready(function() {
  $('#filters').on('click', '.on-sale', function() {
    var tour = $('.tour').filter('.on-sale');
    tour.addClass('highlight');
  });
});
```

**3.23**

```
$(document).ready(function() {
  $('#filters').on('click', '.on-sale', function() {
    $('.tour').filter('.on-sale').addClass('highlight');
    $('.tour').filter('.featured').removeClass('highlight');
  });

  $('#filters').on('click', '.featured', function() {
    $('.tour').filter('.featured').addClass('highlight');
    $('.tour').filter('.on-sale').removeClass('highlight');
  });
});
```

**4.3**

```
$(document).ready(function(){
	alert($('img').length);
});
```

**4.4**

```
$(document).ready(function() {
  $('#tour').on('click','button', function(){
  });
});
```

**4.5**

```
$(document).ready(function() {
  $('#tour').on('click', 'button', function() {
    $('.photos').slideDown();
  });
});
```

**4.6**

```
$(document).ready(function() { 
  $("#tour").on('click', 'button', function() { 
    $('.photos').slideToggle();
  });
});
```

**4.7**

Video

**4.8**

```
$(document).ready(function() {
  $('#tour').on('click', 'button', function() { 
    $('.photos').slideToggle();
  });
  // add a new event handler
  $('.photos').on('mouseenter','li',function(){
  });
});
```

**4.9**

```
$(document).ready(function() {
  $('#tour').on('click', 'button', function() {
    $('.photos').slideToggle();
  });
  $('.photos').on('mouseenter', 'li', function() {
    $(this).find('span').slideToggle();
  });
});
```

**4.10**

```
$(document).ready(function() {
  $('#tour').on('click', 'button', function() {
    $('.photos').slideToggle();
  });
  $('.photos').on('mouseenter', 'li', function() {
    $(this).find('span').slideToggle();
  });
  // add another event handler
  $('.photos').on('mouseleave', 'li', function() {
    $(this).find('span').slideToggle();
  });
});
```

**4.11**

```
$(document).ready(function() {
  $('#tour').on('click', 'button', function() {
    $('.photos').slideToggle();
  });

  // create showPhotos() function
  function showPhotos(){
		$(this).find('span').slideToggle();
  }
    $('.photos').on('mouseenter', 'li', showPhotos);
  	$('.photos').on('mouseleave', 'li', showPhotos);
});
```

**4.13**

```
$(document).ready(function() {
  $('#nights').on('keyup', function (){});
});
```

**4.14**

```
$(document).ready(function() {
  $('#nights').on('keyup', function() {
    $('#nights-count').text($(this).val());
  });
});
```

**4.15**

```
$(document).ready(function() {
  $('#nights').on('keyup', function() {
    $('#nights-count').text($(this).val());
    var nc = +$(this).val();
    var db = +$(this).closest('.tour').data('daily-price');
    $('#total').text(nc*db);
  });
});

```

**4.16**

```
$(document).ready(function() {
  $('#nights').on('keyup', function() {
    var nights = +$(this).val();
    var dailyPrice = +$(this).closest(".tour").data("daily-price");
    $('#total').text(nights * dailyPrice);
    $('#nights-count').text($(this).val());
  });
  // add another event handler
   $('#nights').on('focus', function() {
		$(this).val('7');
  });
});
```

**4.17**

video

**4.18**

```
$(document).ready(function() {
  $('see-photos').on('click', function(){
  
  });
});
```

**4.19**

```
$(document).ready(function() {
  $('.see-photos').on('click', function() {
    $(this).closest('.tour').find('.photos').slideToggle();
  });
});
```

**4.20**

```
$(document).ready(function() {
  $('.see-photos').on('click', function(event) {
    event.stopPropagation();
    $(this).closest('.tour').find('.photos').slideToggle();
  });
  $('.tour').on('click', function() {
    alert('This event handler should not be called.');
  });
});
```

**4.21**

```
$(document).ready(function() {
  $('.see-photos').on('click', function(event) {
    event.stopPropagation();
    event.preventDefault();
    $(this).closest('.tour').find('.photos').slideToggle();
  });
  $('.tour').on('click', function() {
    alert('This event handler should not be called.');
  });
});
```

**5.2 Taming CSS**

```

```

**5.3 CSS I**

```
$(document).ready(function() {
  $('.tour').on('mouseenter', function() {
    $(this).css('background-color', '#252b30');
  });
});
```

**5.4 CSS II**

```
$(document).ready(function() {
  $('.tour').on('mouseenter', function() {
    $(this).css({'background-color':'#252b30','font-weight':'bold'});
  });
});
```

**5.5 Show Photo**

```
$(document).ready(function() {
  $('.tour').on('mouseenter', function() {
    $(this).css({'background-color': '#252b30', 'font-weight': 'bold'});
    $(this).find('.photos').show();
  });
});

```

**5.6 Refactoring to CSS**

```
$(document).ready(function() {
  $('.tour').on('mouseenter', function() {
    $(this).addClass('highlight');
    $(this).find('.photos').show();
  });
  // add a new event handler
  $('.tour').on('mouseleave', function() {
    $(this).removeClass('highlight');
    $(this).find('.photos').show();
  });
});
```

**5.7 Animation**

```

```

**5.8 Animate I**

```
$(document).ready(function() {
  $('.tour').on('mouseenter', function() {
    $(this).addClass('highlight');
    $(this).find('.per-night').animate({'opacity': '1'});
  });
  $('.tour').on('mouseleave', function() {
    $(this).removeClass('highlight');
  });
});
```

**5.9 Animate II**

```
$(document).ready(function() {
  $('.tour').on('mouseenter', function() {
    $(this).addClass('highlight');
    $(this).find('.per-night').animate({'top': '-14px','opacity': '1'},'fast');
  });
  $('.tour').on('mouseleave', function() {
    $(this).removeClass('highlight');
  });
});
```

**5.10 Animation Speed**

```
$(document).ready(function() {
  $('.tour').on('mouseenter', function() {
    $(this).addClass('highlight');
    $(this).find('.per-night').animate({'top': '-14px','opacity': '1'},'fast');
  });
  $('.tour').on('mouseleave', function() {
    $(this).removeClass('highlight');
  });
});
```

**5.11 Animate III**

```
$(document).ready(function() {
  $('.tour').on('mouseenter', function() {
    $(this).addClass('highlight');
    $(this).find('.per-night').animate({'top': '-14px', 'opacity': '1'}, 'fast');
  });
  $('.tour').on('mouseleave', function() {
    $(this).removeClass('highlight');
    $(this).find('.per-night').animate({'top': '0', 'opacity': '0'}, 'fast');
  });
});
```

## Vocabulaire

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
