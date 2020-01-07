# Blog mit Hugo

Zuerst eine Anleitung, wie man neue Inhalte auf der Website speichert. Weiter unten sind zusätzliche Infos zu den verschiedenen Plattformen und zur Software, welche bei der Website involviert sind.


## Anleitung für neuen Inhalt auf der Website

1. **Visual Studio Code** (VS Code) öffnen.
2. Den Ordner mit dem Projekt öffnen (falls das Projekt noch nicht auf dem PC ist, mit der GitHub Desktop App vom eigenen GitHub herunterladen).
3. Im Projekt den Inhalt ändern. Für einen neuen Blogeintrag am besten einen bestehenden Ordner in `/content/blog/...` kopieren und unter neuem Namen einfügen. Dann Titel, Datum, Inhalt und Bilder ändern.
4. **GitHub Desktop** öffnen. Dort sollten die Änderungen sichtbar sein und können überprüft werden.
5. Eine (beliebige) "Summary" für die Änderung eingeben. Dann auf `Commit` klicken. 
6. Schliesslich noch auf den `Push`-Knopf klicken. Der Rest geht automatisch:
    * Code wird auf GitHub hochgeladen.
    * Netlify merkt, dass etwas geändert hat und holt sich den neusten Code.
    * Netlify generiert die Seite mit Hugo und setzt sie Live.
    

## Änderungen Lokal anschauen mit Hugo

Es empfiehlt sich, jeweils die Änderungen lokal im Browser anzuschauen, bevor man es auf GitHub hochlädt. So geht das:

1. In VS Code das Terminal öffnen (Menu `View->Integrated Terminal`).
2. Im Terminal `hugo server` eingeben.
    * Um zukünftige (FUTURE) Blog Posts anzuzeigen: `hugo server -F`
    * Um Entwürfe (DRAFTS) anzuzeigen `hugo server -D`
3. Jetzt im Browser http://localhost:1313/ öffnen (Link wird auch im Terminal angezeigt).
4. Mit Ctrl+C stoppen.


**Hinweis:** Falls mal eine Änderung nicht angezeigt wird (z.B. nach Bearbeiten eines Bildes), dann kann man mit `control+c` Hugo stoppen. Dann mit `Pfeil-hoch` den Befehl `hugo server` nochmals starten.


## Domains

Evtl. bei einem Domainverwalter eine eigene Domain kaufen und mit dem Projekt auf Netlify verknüpfen.


## GitHub

Der Programmcode liegt auf GitHub.com. Bei jeder Änderung, welche auf GitHub eingecheckt wird, wird Netlify aktiviert und aktualisiert die Seite.


## GitHub Desktop

GitHub Destkop ist ein Programm auf dem Mac, mit welchem man neuen Programmcode bei GitHub einchecken (d.h. hochladen) kann.

Download: https://desktop.github.com/


## Netlify

* https://www.netlify.com/
* User: Login mit GitHub-Login.

Auf Netlify ist die Website gehostet. Netlify macht aber mehr als nur Hosting. Netlify lädt den neusten Code von GitHub, sobald etwas geändert hat. Dann führt Netlify das Generieren mit Hugo durch und aktualisiert die Website. Ausserdem ist Netlify zuständig für HTTPS-Zertifikate und für die Weiterleitung aller alternativen Domainnamen.


## Hugo

* https://gohugo.io/documentation/

Hugo muss auf dem PC installiert sein. Falls noch nicht installiert, hier herunterladen: https://github.com/gohugoio/hugo/releases (oberste Version nehmen mit EXTENDED und Windows 64 oder Mac im Namen).

Hugo ist unsere Software, um die Website zu erstellen. Es ist ein Static Site Generator. Hugo nimmt alle Content-Dateien und fügt sie in HTML-Vorlagen ein. Damit hat man am Schluss nur noch HTML und CSS und keine "komplizierten" Sachen mit Datenbank und so auf dem Server.


## Bootstrap

Die Vorlage basiert auf dem Design-Framework von Bootstrap: https://getbootstrap.com/


## Terminal

Das Terminal wird verwendet, um Hugo zu starten. Man kann das normale Mac-/Windows-Terminal nehmen oder - wie oben beschrieben - das integrierte Terminal in Visual Studio Code.


## Autor

✨ [Marco Jakob](https://www.jakob.services)