# Leccion20-Ejercicio2
**Problema1**

var feature = 'closures'; 
(function () {     
	if ( typeof feature === 'undefined' ){         
		var feature = 'callbacks';         
		console.log('JS coders love its ' + feature );     
	} else {         
		console.log('JS developers love its ' + feature );     
	} 
})();

**Solución**

> var feature = 'closures'; 
(function () {     
	if ( typeof feature === 'undefined' ){       
		feature = 'callbacks';
		console.log('JS coders love its ' + feature );     
	} else {         
		console.log('JS developers love its ' + feature );     
	} 
})();

**Explicación**
En el ejemplo propuesto existen dos variables con el mismo nombre pero diferente ambito, en este caso se espera mostrar el mensaje 
**JS developers love its closures.** pero no se obtiene ese resultado por que predomina la variable local , en la condición se lee la variable feature aunque no este inicializada por eso la pasa como undefined , pero igual la lee y muestra el mensaje.
La solución fue dejar la variable global para que cuando pase por la condición sea falsa y muestre el mensaje esperado.
La solución para este caso fue eliminar la variable local para poder tomar la global feature = 'closures'

