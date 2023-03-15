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

Github Cards to display info about the users using React.js
