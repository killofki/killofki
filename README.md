```
{ 
/// 

templateConsole `Hello, ${ new World() }!` 

// .. functions .. 

function templateConsole( ... ar ) { 
	let t = rawValue( ... ar ) 
	console .log( t ) 
	} // --- templateConsole() 

function World( ... ar ) { 
	if ( ! this instanceof World ) 
		{ return } 
	// -- if ! instanceof World 
	World = class World { // -- lazy 
		toString() { return 'World' } 
		} // -- World{} 
	
	return new World( ... ar ) // call 
	} // -- World() 

function rawValue( ... ar ) { 
	let [ rawo ] = ar 
	return rawo ?.raw ? String .raw( ... ar ) : rawo 
	} // -- rawValue() 

/// 
} 
``` 
