# Github-Cards
- https://jscomplete.com/playground/rgs2.1
- https://jscomplete.com/playground/rgs2.2
- https://jscomplete.com/playground/rgs2.3
- https://jscomplete.com/playground/s907652 
- When we use spread operator with an oject like this in react component , all the properties of the object will become props of that component, where testdata is a json to define properties like name,email and age of an object 

```
const CardList = (props) => (
	<div>
  	<Card {...testData[0]} />
        <Card {...testData[1]} />
	</div>
);

```

- Instead of hardcoding the values in the card element, whjat we need to do is to take an array of objects  as in the testdata array and map it into an array of card elements. To parse the values dynamically from json , 

```
const CardList = (props) => (
	<div>
  	{testData.map(profile => <Card {...profile}/>)}
	</div>
);
```
- https://jscomplete.com/playground/rgs2.4
- map() takes a function as an argument & converts one array to another array using the return values in the function
```
[<Card /><Card />,<Card />]
// It will render an array of card elements 
[React.createElement(),React.createElement(),React.createElement()]
```
- https://jscomplete.com/playground/rgs2.4
  - Add an input box and log the value using Refs 
  - https://jscomplete.com/playground/s907660
  
- https://jscomplete.com/playground/rgs2.5


Github Cards to display info about the users using React.js
