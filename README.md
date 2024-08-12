Watch this in Youtube:

[![Watch the video](https://img.youtube.com/vi/2gLufgeYnZ4/hqdefault.jpg)](https://www.youtube.com/embed/2gLufgeYnZ4)

# Einführung

Dies ist eine Projektmanagement-Software, die mit Qt / C++ geschrieben wurde und durch die Verbindung mit einer SQL-Datenbank funktioniert.

Es können Projekte hinzugefügt, gelöscht, bearbeitet und abgefragt werden. Es enthält eine Konsole, die direkte SQL-Abfragebefehle akzeptiert.

Es kann zwischen Deutsch und Englisch gewechselt werden, die Wahl des Benutzers wird automatisch in der Windows-Registrierung gespeichert und beim nächsten Start automatisch aus der Registrierung gelesen.

Ich habe das Projekt eigenständig in 4 Tagen abgeschlossen.

## GUI

### Hauptoberfläche
Hauptoberfläche besteht aus:

"Neu Projekt": Anlegen neuer Projekte,

"Projekt Info": Anzeigen und Abändern vorhandener Info, die für Benutzer relevant ist,

"Daten Holen": alle Änderungen werden zur SQL-Datenbank versendet,

"SQL Studio": eingebettete SQL Query Konsole, mit SQL Syntax Daten aus Datenbank abfragen (Query only),

"Deutsch", "Englisch": Sprache wechseln zwischen Deutsch und Englisch,

"Unerledigt": Anzeigen aller neu angelegten Projekte, die noch nicht in Arbeit sind,

"in Arbeit": Anzeigen aller Projekte, die schon begonnen sind und noch nicht fertig sind,

"Erledigt": Anzeigen aller Projekte, die schon fertig sind. Alle erledigten Projekte sollen in "Projekt Info" nicht angezeigt werden, aber in der SQL-Datenbank als erledigt markiert werden.

"Beenden": Beenden des Programms

![image](https://github.com/user-attachments/assets/12aa95e5-6d13-494f-a9fb-23554d8b1792)

---

### Unteroberfläche "Neu Projekt"

"ID": nächste mögliche Nummer wird automatsch suggiert,
"Bezeichnung": Eingabe Projektname und name wird über "Regular Expression" überprüft,
"Speichern": Daten wird von Software übernommen.

![image](https://github.com/user-attachments/assets/c1ee6cc0-7eae-4250-a64a-1c5ce414137c)

---

### Unteroberfläche "Projekt Info"

Anzeigen und Abändern vorhandener Info, die für Benutzer relevant ist.

"Projektname": jeder Änderung wird über "Regular Expression" überprüft,

"Startdatum": Datum kann nur aus eine Kalender ausgewählt wird, um Fehreingabe zu vermeiden,

"Bemerkung": alle Stringformat wird hier akzeptiert,

"ID" und "Stauts": hier wird keine Änderung akzeptiert,

"Hochladen": alle Änderungen werden zur SQL Datenbank hochgeladen,

"Undo_All": alle Änderungen werden wiederhergestellt.

![image](https://github.com/user-attachments/assets/1a1dc56b-165a-4b34-9a42-17b4622c5679)

---

### Unteroberfläche "SQL Studio"

Eingebettete SQL Query Konsole, mit SQL Syntax Daten aus Datenbank abfragen (Query only),

![image](https://github.com/user-attachments/assets/2b3d2cac-f65c-43bc-bbce-345685d49c82)

---
