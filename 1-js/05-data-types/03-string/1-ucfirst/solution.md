In JavaScript ist es nicht möglich, das erste Zeichen eines Strings zu "ersetzen", da diese nicht veränderbar sind.

Jedoch ist es möglich, einen neuen String zu erzeugen, welcher auf den existierenden aufbaut, jedoch mit einem großen Anfangsbuchstaben anfängt.

```js
let newStr = str[0].toUpperCase() + str.slice(1);
```

Hier ist jedoch ein Problem: Wenn `str` leer ist, gilt `str[0]` als `undefined` und enthält somit keine Methode `toUpperCase()`, wodurch wir einen Error erhalten würden.

Dafür gibt es zwei verschiedene Lösungswege:

1. Nutzen von `str.charAt(0)`, da es immer einen String zurückgibt, welcher auch leer sein kann.
2. Hinzufügen einer Abfrage, ob der String leer ist.

Hier ist die **zweite** Methode:

```js run demo
function ucFirst(str) {
  if (!str) return str;

  return str[0].toUpperCase() + str.slice(1);
}

alert( ucFirst("john") ); // John
```
