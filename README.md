
An arrow function example:

(someArg) => {
	// Do stuff
	return someValue;
}

Arrow functions have three benefits:

* Much more concise
* They have implicit returns (for functions with only a return statement)
* They don't rebind the value of this

Notes: 

* All arrow function are anonymous, meaning they will not show up on a 
  stack trace.
* If implicit return is used, don't specify the brackets or return.
* We can assign a function to a variable.

const fullNames = names.map(name => `${name} cool`);

/*** Another example, note we could use parenthesis to create an implicit return ***/

const win = winners.map((winner, i) => {
	return {
		name: winner,
		race: race,
		place: i
	}
})