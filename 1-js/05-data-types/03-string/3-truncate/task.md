importance: 5

---

# Text kürzen


Schreibe eine Funktion `truncate(str, maxlength)` welche die Länge des Strings `str` prüft und, wenn er länger als `maxlength` ist -- das Ende von `str` mit dem Auslassungszeichen `"…"` so ersetzt, das die insgesamte Länge des Strings nicht länder als `maxlength` ist.

Das Ergebnis der Funktion sollte der gekürzte String mit, sofern benötigt, dem Auslassungszeichen sein.

Beispielsweise:

```js
truncate("Was ich dir in über dieses Thema gerne erzählen würde:", 20) = "Was ich dir in über…"

truncate("Hallo zusammen!", 20) = "Hallo zusammen!"
```
