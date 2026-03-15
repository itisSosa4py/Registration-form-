nicht sehr besonders logik in diese projekt , ein normale anmeldung form . 

"function login(a) {
    console.log(a)
}

function submit() {
    console.log("ram")
    const name = document.getElementById("name").value
    const Surname = document.getElementById("Surname").value
    const Age = document.getElementById("Age").value
    const Gender = document.getElementById("Gender").value
    const DOB = document.getElementById("DOB").value
    const Email = document.getElementById("E-mail").value
    const Website = document.getElementById("Website").value
    console.log(name.trim())
    console.log(Surname.trim())
    console.log(Age.trim())
    console.log (Gender.trim())
    console.log  (DOB.trim()) 
    console.log(Email.trim())
    console.log (Website.trim())
    
}"
### Logik des JavaScript-Codes (Formularverarbeitung)

Dieser JavaScript-Code dient dazu, **Benutzereingaben aus einem HTML-Formular auszulesen und in der Browser-Konsole auszugeben**. Er besteht aus zwei Funktionen: `login()` und `submit()`.

---

#### 1. Funktion `login(a)`

```javascript
function login(a) {
    console.log(a)
}
```

**Logik:**

* Die Funktion erhält einen **Parameter `a`**.
* Dieser Wert wird mit `console.log()` in der **Browser-Konsole** ausgegeben.
* Sie dient hauptsächlich zu **Debugging-Zwecken oder zum Testen von Eingabewerten**.

---

#### 2. Funktion `submit()`

```javascript
function submit() {
    console.log("ram")
}
```

Diese Funktion wird typischerweise **beim Absenden eines Formulars** aufgerufen.

---

#### 3. Auslesen der Eingabefelder

```javascript
const name = document.getElementById("name").value
```

**Logik:**

* `document.getElementById()` greift auf ein **HTML-Element mit einer bestimmten ID** zu.
* `.value` liest den **vom Benutzer eingegebenen Wert** aus dem Formularfeld.

Dieser Vorgang wird für mehrere Felder wiederholt:

* Name
* Surname
* Age
* Gender
* DOB (Date of Birth)
* E-mail
* Website

Alle Werte werden in **Variablen gespeichert**.

---

#### 4. Verwendung von `.trim()`

```javascript
console.log(name.trim())
```

**Logik:**

* `.trim()` entfernt **Leerzeichen am Anfang und Ende eines Strings**.
* Dadurch werden Eingaben wie `"  Max "` zu `"Max"` bereinigt.
* Dies verhindert Probleme bei **Validierung oder Datenverarbeitung**.

---

#### 5. Ausgabe in der Konsole

```javascript
console.log(...)
```

Alle bereinigten Werte werden anschließend in der **Browser-Konsole ausgegeben**.
Dies hilft Entwicklern dabei, zu überprüfen, ob die **Formulardaten korrekt gelesen wurden**.

---

### Ergebnis

Die Funktion `submit()`:

1. Liest mehrere **Eingabewerte aus einem HTML-Formular**.
2. Entfernt unnötige **Leerzeichen mit `.trim()`**.
3. Gibt die bereinigten Daten zur **Kontrolle in der Konsole** aus.

Diese Technik wird häufig verwendet, um **Formulardaten zu überprüfen oder weiterzuverarbeiten**, bevor sie z. B. an einen Server gesendet werden.
