Entwurf Nextcloud Video Converter Javanauts Fork

v1.1.0

Job-Tabelle

http://jsfiddle.net/venkateshwar/5KJka/1/

Start:
  Jobliste einlesen
  Tabelle aktualisieren
  Auf PID file prüfem:
      Auf Worker prüfen:
          Worker Starten
          
Delete:
  Jobs von Liste streichen
  Tabelle aktualisieren
  
Cancel: Worker abschiessen
  Jobs von Liste streichen
  Tabelle aktualisieren
  Worker starten

Codec:
   h264
   HEVC
   h264 (2-Pass) -> Verfügbar wenn x264 entdeckt wurde

Bitrate:
   Absolut in kbit/s
   Relativ in % des Originalfiles

Output format:
   .MKV verfügbar wenn mkvtoolnix entdeckt

Add Job:
    Fügt ausgewählte Dateien und Parameter zu Job-File hinzu
    Liest Job-File ein und aktualisiert angezeigte Job-Liste
    Prüft ob Worker-Prozess aktiv ist
    Startet / startet neu PHP-Worker-Prozess 
    
Worker:
    PID File erzeugen
    Jobfile einlesen
    Konvertierung starten
    Jobfile aktualisieren
        Nächste Konvertierung starten
    Tempfiles löschen
    Jobfile und PID File löschen