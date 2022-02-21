```
{ 
/// 

templateConsole `Hello, ${ new World() }!` 

// .. functions .. 

function templateConsole( ... ar ) { 
	let t = rawValue( ... ar ) 
	console .log( t ) 
	} // --- templateConsole() 

function World() { 
	if ( ! this instanceof World ) 
		{ return } 
	// -- if ! instanceof World 

	return new class World { 
		toString() { return 'World' } 
		} // -- World{} 
	} // -- World() 

function rawValue( ... ar ) { 
	let [ rawo ] = ar 
	return rawo ?.raw ? String .raw( ... ar ) : rawo 
	} // -- rawValue() 

/// 
} 
``` 
