# LB 324

## Aufgabe 2
Erklären Sie hier, wie man `pre-commit` installiert.
1.  Installation
        Installiere alle benötigten Pakete aus der requirements.txt
        pip install -r requirements.txt

2.  Hooks aktivieren
        pre-commit install
        pre-commit install --hook-type pre-push

3.  Automatischer Ablauf im Workflow
        Bei jedem git commit läuft automatisch black zur Formatierung des Codes.
        Bei jedem git push werden automatisch die Tests (pytest) ausgeführt. Schlägt ein Test fehl, wird der push abgebrochen.
        
## Aufgabe 4
Erklären Sie hier, wie Sie das Passwort aus Ihrer lokalen `.env` auf Azure übertragen.

Damit der Login auch auf Azure funktioniert, muss die Umgebungsvariable PASSWORD
manuell als App-Einstellung in Azure hinterlegt werden.

1. Im Azure-Portal die Web-App öffnen.
2. Links im Menü Settings Environment variables wählen.
3. Add klicken, Name PASSWORD, Wert eintragen.
4. Mit Apply/Save speichern, die Web-App startet danach neu.
