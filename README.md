# django_project_templates
Schablonen, um Django-Anwendungen zu generieren.

Leistungsmerkmale (Grundfunktionen bei der Generierung eines neuen Projektes):
  - benutzerdefiniertes Benutzermodell.
  - bootstrap-Integration.
  - jquery-Integration.
  - popper-Integration.
  - chartjs-Integration.
  - scss-basierte Stildefinitionen (CSS), Kompilierung über einen einfachen make-Befehl.
  - einfach verschachtelte HTML-Schablonen für die Seiten (templates).
  - Menübaum.
  - cache_bust für effektives Weiterentwickeln integriert (abschaltbar).
  - simple_history integriert.
  
Leistungsmerkmale (Funktionen beim Hinzufügen von Klassen):
  - Erzeugen von Klassenkörpern für Tabellen (models).
  - Erzeugen von sinnvollen Einträgen für die django-admin Schnittstelle (Einträge in admin.py).
  
Installation:

  - Herunterladen der Projektschablonen
  - Erzeugen eines Django-Projektes mit Hilfe der Schablonen:
  
  django-admin startproject --template "Pfad zu der Projektschablone" "Projektname"

  - Ins Projektverzeichnis wechseln und make eingeben, um die CSS-Dateien zu generieren.
  - Mit pip install -r requirements.txt Abhängigkeiten installieren
  - Migrationen erzeugen
  - Migrationen anwenden
  - Mit python manage.py runserver Projekt starten

Hinzufügen von Klassen:

  python manage.py startmodul --help
  
  python manage.py startmodul --kuerzel "Präfix für kurze SQL-Feldnamen (3 Stellen empfohlen)" --klassname "Klassenname für die Tabelle"
  
 Damit wird ein neues Modul erzeugt (django-app), und darin eine Klasse mit Admin-Schnittstelle angelegt.
 
 Die neu erzeugte django-app muß noch von Hand in der setting.py-Datei eingetragen werden, um berücksichtigt zu werden.
 
 Warnung: Das Projekt verwendet Schriftarten (als Kopien dauerhaft im generierten Projektverzeichnis abgelegt) von Christian Robertson, welche der Apache Lizenz unterliegen.

Das Projekt bettet direkt verschiedene weitere Dateien von fremder Software ein (bootstrap, jquerey, popper, chartjs uws.), welche jeweils ihren eignen Lizenzen unterliegen.

Es werden während des Betriebes eines auf diesen Schablonen basierenden Projektes KEINE Dateien von externen Servern beim Benutzer nachgeladen - deswegen werden Kopien vorgehalten und aus dem static-Verzeichnis der Anwendung direkt ausgeliefert. Dies erhöht die Stabilität der Anwendungen (weniger Abhängigkeiten von externen Resourcen.)
