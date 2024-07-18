# Lern-Bericht

## Einleitung

In den Sommerferien habe ich begonnen, die Programmiersprache Python zu lernen. 🐍

## Was habe ich gelernt?

Ich habe gelernt, wie man mathematische Ausdrücke in Python auswertet und einfache Fehlerbehandlung implementiert. 🧮

## Beschreibung

Ich habe mithilfe von [w3schools](https://www.w3schools.com/python/) mir die Grundkenntnisse von Python angeeignet und beschlossen, einen Taschenrechner zu programmieren, der komplette Rechnungen wie `1 + 1` oder `3 - 2 + 1` verarbeiten kann, um zu überprüfen, ob ich alles verstanden habe.

Hier ist der Code, den ich verwendet habe, und eine Erklärung der einzelnen Teile:

### 1. Funktion zur Berechnung von Ausdrücken

```python
def calculate(expression):
    try:
        # Die eval()-Funktion wird verwendet, um den mathematischen Ausdruck zu berechnen.
        result = eval(expression)
        return result
    except Exception as e:
        return f"Fehler: {str(e)}"
```

**Erklärung:**
- **`def calculate(expression):`**: Definiert eine Funktion namens `calculate`, die einen Parameter `expression` erhält, welcher den mathematischen Ausdruck als String enthält.
- **`result = eval(expression)`**: Verwendet die `eval()`-Funktion, um den mathematischen Ausdruck auszuwerten.
- **`return result`**: Gibt das Ergebnis der Berechnung zurück.
- **`except Exception as e:`**: Fängt alle Ausnahmen, die während der Auswertung auftreten könnten.
- **`return f"Fehler: {str(e)}"`**: Gibt eine Fehlermeldung zurück, wenn ein Fehler auftritt.

### 2. Benutzerinteraktion und Berechnung

```python
print("Geben Sie einen mathematischen Ausdruck ein (z.B. 1 + 1):")
expression = input("Rechnung: ")

# Ergebnis berechnen und ausgeben
result = calculate(expression)
print(f"Ergebnis: {result}")
```

**Erklärung:**
- **`print("Geben Sie einen mathematischen Ausdruck ein (z.B. 1 + 1):")`**: Fordert den Benutzer auf, einen mathematischen Ausdruck einzugeben.
- **`expression = input("Rechnung: ")`**: Liest die Benutzereingabe und speichert sie in der Variablen `expression`.
- **`result = calculate(expression)`**: Ruft die `calculate`-Funktion auf, um das Ergebnis des eingegebenen Ausdrucks zu berechnen.
- **`print(f"Ergebnis: {result}")`**: Gibt das Ergebnis der Berechnung aus.

## Reflektion zum Arbeitsprozess

👍 Ich war sehr motiviert und habe schnell die Grundkenntnisse erlernt.

👎 Allerdings hat es mich frustriert, dass es nicht auf Anhieb funktionierte.

**Verbesserungsvorschläge (VBV):** Da ich alles an einem Tag gelernt habe, war der Lerneffekt nicht so gross. Beim nächsten Mal werde ich das Lernen auf mehrere Tage verteilen und auch Pausen einlegen, um den Lernprozess zu optimieren. ⏳
