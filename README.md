```
{ /// 

templateConsole `Hello, ${ new World() }!` 

// .. functions .. 

function templateConsole( ... ar ) { 
	const t = rawValue( ... ar ) 
	console .log( t ) 
	} // --- templateConsole() 

function World( ... ar ) { 
	World = class World extends String { // -- lazy 
		constructor( ... ar ) { 
			const { length } = ar 
			if ( ! length ) { 
				ar = [ 'World' ] 
				} // -- if ! length 
			super( ... ar ) 
			} // -- constructor() 
		} // -- World{} 
	
	return new World( ... ar ) // call 
	} // -- World() 

function rawValue( ... ar ) { 
	const [ rawo ] = ar 
	return rawo ?.raw ? String .raw( ... ar ) 
		: rawo 
	} // -- rawValue() 

} /// 
``` 
