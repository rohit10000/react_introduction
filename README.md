## Intro to React: [link](https://reactjs.org/tutorial/tutorial.html)

### Prerequisites
- familiarity with HTML and JavaScript
- programming concepts like functions, objects, arrays, and to a lesser extent, classes.
- some features from ES6( arrow functions, classes, let, and const statements)

### Goal:
- Lets you play tic-tac-toe,
- Indicates when a player has won the game,
- Stores a game’s history as a game progresses,
- Allows players to review a game’s history and see previous versions of a game’s board.

### Learning:
	- React elements
	- components
	- props
	- state
	- handson
	

### What Is React?
- React is a declarative, efficient, and flexible JavaScript library for building user interfaces.
It lets you compose complex UIs from small and isolated pieces of code called “components”.

<b><i>Note</i></b>:
	In JavaScript classes, you need to always call super when defining the constructor of a subclass. 
	All React component classes that have a constructor should start with a super(props) call.

<b><i>Note</i></b>:
	Since the Square components no longer maintain state, the Square components receive 
	values from the Board component and inform the Board component when they’re clicked. 
	In React terms, the Square components are now controlled components. The Board has full 
	control over them.
	
### Why Immutability Is Important?
we suggested that you create a copy of the squares array using the slice() 
method instead of modifying the existing array.

```
Data Change with Mutation
	eg.
		var player = {score: 1, name: 'Jeff'};
		player.score = 2;
		// Now player is {score: 2, name: 'Jeff'}
		
Data Change without Mutation
	eg.
		var player = {score: 1, name: 'Jeff'};

		var newPlayer = Object.assign({}, player, {score: 2});
		// Now player is unchanged, but newPlayer is {score: 2, name: 'Jeff'}

		// Or if you are using object spread syntax proposal, you can write:
		// var newPlayer = {...player, score: 2};

```

<b><i>Note:</i></b>
	When we modified the Square to be a function component, we also changed 
	onClick={() => this.props.onClick()} to a shorter 
	onClick={props.onClick} (note the lack of parentheses on both sides).

<b><i>Note:</i></b>
	Unlike the array push() method you might be more familiar with, 
	the concat() method doesn’t mutate the original array, so we prefer it.


		
### Helpful link:
- https://reactjs.org/docs/optimizing-performance.html#examples
- https://reactjs.org/docs/state-and-lifecycle.html#state-updates-are-merged