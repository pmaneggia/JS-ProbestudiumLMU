# JavaScript Übersicht 

Syntax ähnlich wie Java und C, objektorientiert, funktional, prototypische Vererbung, dynamisch typisiert.

## Kommentare
```javascript
// einzeilig
/* mehrzeilig: Zeile 1
Zeile 2 */
```

## Variablen
```javascript
x = 3; // global
let x = 3; // lokal
var x = 3; // lokal (altmodisch)
const X = 3; // Konstante
```

## Datentypen

Die wichtigste Datentypen sind:

* [Number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number) - 64-Bits double precision floating number, keine ganze Zahl!
* [String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)
* [Boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean) - true, false
* [Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)
  * [Array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)
  * [Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function)
  
Datentypen sind auch:

* [null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)
* [undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)
* [Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date)
* [RegExp](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/RegExp) - Regulärer Ausdruck
* [Symbol](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Symbol) 

Beispiele und wichtigste Operatoren

```javascript
let n = 0.5; // Number
// +, -, *, /
Math.floor(n); // abrunden 
Math.pow(b,e); // Potenz: b hoch e
Math.abs(n); // Betrag
n % d; // Modulo-Operator: Rest der ganzahligen Division
NaN // Wert <Not a Number> falls nicht auf eine Zahl zurückzuführen

// String
let s = 'Hallo'; // oder auch: "Hallo";
s + ' Welt!'; // -> 'Hallo Welt!' 
s.length; // -> 5
s.charAt(1); // -> 'a'

// Boolean
let b = true;
false;
//boolesche Operatoren
x === y; // ist gleich
x !== y; // ist ungleich
x < y; // ist kleiner
x <= y // ist kleiner oder gleich
x > y; // ist größer
x >= y // ist größer oder gleich
!b; // Verneinung
b && c; // und
b || c; // oder

//Objekt
let o = {l: 3, r: 5, f: function(x) {return this.l <= x && x <= this.r;}};
o.l; // -> 3
o.f(4.6); // -> true 

//Array
let obst = ['Apfel', 'Kokosnuss', 'Birne'];
obst[0]; // -> 'Apfel'
obst.length; // -> 3;
//Arrays in Javascript können Objekte von verschiedenen Datentypen enthalten
let mix = [5.3, 'Tokyo', false, [7,6,5]];
//Viele interessante Methoden: includes(x), indexOf(x), join(), map(), pop(), push(), ...

//Function: s. nächste Abschnitt
```

## Funktionen

Funktionen in Javascript sind selbst Objekte! 
Die Syntax für die Definition einer Funktion ist:

```js
function summe(x, y) {
 return x + y;
}
```
// oder
```js
summe = (x, y) => {
 return x + y;
}
```

## Debugging
```js
console.log("Hallo Welt");
```
oder in Browser-Debugger

