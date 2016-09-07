# Leccion20-Ejercicio2
_Ejemplo_
var feature = 'closures'; 
(function () {     
	if ( typeof feature === 'undefined' ){         
		var feature = 'callbacks';         
		console.log('JS coders love its ' + feature );     
	} else {         
		console.log('JS developers love its ' + feature );     
	} 
})();

> Solución
var feature = 'closures'; 
(function () {     
	if ( typeof feature === 'undefined' ){         
		console.log('JS coders love its ' + feature );     
	} else {         
		console.log('JS developers love its ' + feature );     
	} 
})();


