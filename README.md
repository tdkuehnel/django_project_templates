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
  
  django-admin startproject --template <Pfad zu der Projektschablone> <Projektname>

  - Ins Projektverzeichnis wechseln und make eingeben, um die CSS-Dateien zu generieren.
  - Mit pip install -r requirements.txt Abhängigkeiten installieren
  - Migrationen erzeugen
  - Migrationen anwenden
  - Mit python manage.py runserver Projekt starten