```
{ /// 

templateConsole `Hello, ${ new World() }!` 

// .. functions .. 

function templateConsole( ... ar ) { 
	const t = rawValue( ... ar ) 
	console .log( t ) 
	} // --- templateConsole() 

function World( ... ar ) { 
	const originWorld = World 
	
	World = class World extends String { // -- lazy 
		constructor( ... ar ) { 
			ar .length ? super( ... ar ) : super( 'World' ) 
			} // -- constructor() 
		} // -- World{} 
	
	switch( true ) { 
		case this instanceof originWorld : 
			return new World( ... ar ) // call 
		
		case World === originWorld : 
			throw 'not completed lazy about assign class World' 
		
		default : 
			return World( ... ar ) // call 
		} // -- switch true 
	
	} // -- World() 

function rawValue( ... ar ) { 
	const [ rawo ] = ar 
	return rawo ?.raw ? String .raw( ... ar ) 
		: rawo 
	} // -- rawValue() 

} /// 
``` 
