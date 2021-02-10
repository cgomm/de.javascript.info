Die maximale Länge muss `maxlength` sein, also benötigen müssen wir den String etwas verkürzen, um Platz für das Auslassungszeichen zu erhalten.

Beachte, dass es sich dabei um ein eigenes Unicode Zeichen handelt ('…', U+2026 Horizontal Ellipsis). Es sind **keine** drei Punkte.

```js run demo
function truncate(str, maxlength) {
  return (str.length > maxlength) ?
    str.slice(0, maxlength - 1) + '…' : str;
}
```
