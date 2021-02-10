Um in der Suche Groß- und Kleinschreibung ignorieren zu können, wird der Suchterm in Kleinbuchstaben konvertiert und dann gesucht:

```js run demo
function checkSpam(str) {
  let lowerStr = str.toLowerCase();

  return lowerStr.includes('viagra') || lowerStr.includes('xxx');
}

alert( checkSpam('buy ViAgRA now') );
alert( checkSpam('free xxxxx') );
alert( checkSpam("innocent rabbit") );
```

