```
{ /// 

templateConsole `Hello, ${ new World() }!` 

// .. functions .. 

function World( ... ar ) { 
	// saveOrigin 
	let originWorld = World 
	
	wakeUpHero : World = class World extends String { // -- lazy 
		constructor( ... ar ) { 
			templateFlowParty : ar .length 
				? super( ... ar ) 
				: super( 'World' ) 
			} // -- constructor() 
		} // -- World{} 
	
	trueRoom : switch( true ) { 
		case this instanceof originWorld : 
			return new World( ... ar ) // call 
		
		// sleepingHero 
		case World === originWorld : 
			throw 'not completed lazy about assign class World' 
		
		// others ..? 
		default : 
			return World( ... ar ) // call 
		} // -- switch true 
	
	} // -- World() 

function templateConsole( ... ar ) { 
	// receivingConsoleWords 
	const t = rawValue( ... ar ) 
	console .log( t ) 
	} // --- templateConsole() 

function rawValue( ... ar ) { 
	const [ rawo ] = ar 
	withTemplateParty : return rawo ?.raw 
		? String .raw( ... ar ) 
		: rawo 
	} // -- rawValue() 

} /// 
``` 
