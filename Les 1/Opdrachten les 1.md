*Opdracht 1.1: No jQuery**  
In 2tallen: Noteer voor- en nadelen van jQuery (minimaal 5 van ieder)

	Voordelen:
	- Werkt crossbrowser
	- Gecompliceerde Javascript laten werken met weinig code 
	- Grote community
	- Kan makkelijker zijn voor onervaren programmeurs
	- Goede documentatie

	Nadelen:
	- Grote library
	- Veel updates die het (bestaande)gedrag aan kunnen passen
	- Moeilijker om fouten te achterhalen (chaining of code)
	- Code weegt vaak zwaarder dan non-jQuery code
	- Makkelijker te hacken



**Opdracht 1.2: Functionaliteiten jQuery**  
Noem de belangrijkste functionaliteiten van jQuery (minimaal 5)

	1. Eenvoudige navigatie door de DOM
	2. Selectors
	3. Animaties
	4. AJAX interactie met de server
	5. Event listeners



**Opdracht 1.3: Micro libraries**  
Zoek op http://microjs.com naar libraries voor elke van de functionaliteiten gevonden bij opdracht 1.2 
(deel jQuery op in verschillende micro libs). Kies voor elke functie een micro library (vergelijk en beoordeel op kwaliteit)

	1. xui:				DOM library for authoring HTML5 mobile web applications, works cross-device and cross-platform.
	2. JSONSelect:		CSS-like selectors for JSON.
	3. swipe:			A lightweight 1-to-1 mobile slider. Optimized for touch devices.
	4. Zepto:			jQuery API-compatible framework for modern web browsers. Optional Ajax, Events, Data and Touch modules.
	5. atom.js:			Small class providing async control flow, property listeners, barrier pattern, and more. For node and browser.



#####*2: Objects (30 minuten)*
---
**Opdracht 2.1: Constructor object**  
Maak met een object constructor een ‘Persoon’-object aan met de property ‘name’ en de method ‘speak’. En maak een nieuwe instantie aan van dit object waarbij je de naam ‘Bob’ meegeeft als parameter van het object

	function Person(name){
		this.name = name;

		this.speak = function (){
			console.log('Hi my name is' + this.name);
		}
	}
	var bob = new Person('Bob');



**Opdracht 2.2: Prototype**  
Voeg de methods ‘walk’ en ‘eat’ toe aan het ‘Persoon’-object met de prototype function van het object

function Person(name){
		this.name = name;

		this.speak = function (){
			console.log('Hi my name is' + this.name);
		}
	}

	Person.prototype.walk = function () {
	console.log('Hi my name is ' + this.name + " and I walk often.");
}

	Person.prototype.eat = function () {
	console.log('Hi my name is ' + this.name + " and I eat a lot of fruit.");
}

	var bob = new Person('Bob');


**Opdracht 2.3: Object Literal**  
Maak nu hetzelfde object, met dezelfde properties en methods aan met een object literal

var person = {
	name: 'Bob',

	speak: function () {
		console.log('Hi my name is ' + this.name);
	},

	walk: function () {

	},

	eat: function () {

	}
}

person.speak();


#####*3: Scope (30 minuten)*
---
**Opdracht 3.1: Local Scope**  
Maak met behulp van een function een local scope aan en definieer in deze local scope de variables ‘iterator’, ‘max’ en ‘min’ aan

function Person () {
	var iterator = 1;
	var max = 5;
	var min = 0;
}


**Opdracht 3.2: Global Scope**  
Maak dezelfde variables nu ook aan in de global scope

var iterator = 1;
var max = 5;
var min = 0;


**Opdracht 3.3: Closure**  
Leg uit wat een closure is en maak een code voorbeeld




#####*4: Refactoring GEO Script (30 minuten)*
---
**Opdracht 4.1: Breakdown script**
URL: https://github.com/ju5tu5/cmdgeo/blob/master/src/cmdgeo-0.1.js      
Het GEO script is niet gestructureerd en bestaat uit losse (globale) variabelen en functies. Maak op papier een breakdown van het Geo Script. schrijf de verschillende functionaliteiten op en leid er objecten met properties en methods uit af

var gps = {

	init: function () {

	},

	startInterval: function(){

	},

	updatePosition: function(){

	},

	setPosition: function(){,

	},

	checkLocations: function(){

	}, 
}

var maps = {

	generateMap: function(){

	},

	isNumber: function(){

	},

	updatePositie: function(){

	},

}


var debugging = {

	geoErrorHandler: function(){

	},

	debugMessage: function(){

	},

	setCustomDebugging: function(){

	},

}



**Opdracht 4.2: Create objects**    
Werk de breakdown uit in JavaScript  

####Vooruit kijken
Wat hebben we gedaan, waarom? wat heb je geleerd?  
- Als je nog meer wilt:   
	- Codecadamy: Introduction to Objects I - What is an Object  
	- Codecadamy: Project: Building an Adress Book  
- Volgende week: JavaScript & Structuur  


###Eindopdracht

Webapp Score App voor een sporttoernooi.
Met een team van meerdere developers op een gestructureerde manier aan een webapp werken. 
Denk aan code organiseren, versie controle van je app, bugtracking en commenting. 

Al je werk toevoegen aan Github - Social Coding
'Samenwerken' aan je individuele opdracht