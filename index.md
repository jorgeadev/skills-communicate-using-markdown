# Jorge Gomez

How it looks

![Image of Yaktocat](https://octodex.github.com/images/yaktocat.png)

``` javascript
function createMagicPotion(potions, goal) {
	const complement = {};
	for (let i = 0; i < potions.length; i++) {
		const currentElement = potions[i];
		const difference = goal - currentElement;
		if (complement[currentElement] !== undefined) {
			return [complement[currentElement], i];
		}
		complement[difference] = i;
	}
	return undefined;
}
```
