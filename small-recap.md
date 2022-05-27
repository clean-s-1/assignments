# Well-named recap

## Separation of concerns

Form the Reference Manual contents [in its own function `getReferenceManual`](https://github.com/clean-s-1/well-named-in-js-kmzakiya/blob/df38215966cbb8141747fad1e872e74e0c126e40/app/referenceManual.js)

...and exploit off-the-shelf NodeJS functionality for formatting:

```js
console.table(getReferenceManual());
```

## Testing to safeguard functionality

Separation of concerns helps in testability, saving on manual inspection. See `getReferenceManual` above as an example

Catch and fix the spelling issue 'MinorColr' in `toString`. Also think of what a user would expect to see in a string: 'MajorColor'? or 'Major Color'?

```js
ColorPair.prototype.toString = function () {
  return `MajorColor:${this.majorColor},MinorColr:${this.minorColor}`;
};
```

## Name the file to reflect the purpose

Consider a file having functions `getColorFromPairNumber` and `getPairNumberFromColor`: Call it `colorPairTranslator` instead of `colorUtils`

