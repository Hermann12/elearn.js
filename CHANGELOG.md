### Changelog

* __1.0.11__:
  * Changed:
    * On section change the section name is appended as parameter to the URL
    instead of the section index to make it better human readable
  * Fixes:
    * exactly 4:3 images are scaled correctly in the navigation slider of image galleries
    * images in the navigation slider of image galleries are placed correctly
    * unnecessary backgrounds were removed
* __1.0.10__:
  * Fixes:
    * `hover-info` attribute `data-width` can be used without setting `data-full-width`
    * code refactoring, fixing typos, remove unnecessary code
* __1.0.9__:
  * Changed:
    * blockquote elements will only emphasize their first line as heading if
    the class `emph-heading` is present
    * `.hideable` elements can be visible on load with `.visible`
  * Fixes:
    * `.hover-info` blocks are aligned correctly at any size
* __1.0.8__:
  * New:
    * image galleries can be `.back-loop` instead of loop to jump to the actual first/last image
    * `hover-info` can now be `.full`, to support more dynamic width
    * `fixed-size` for image galleries can now be set on the `div.slider`
* __1.0.7__:
  * Fixes:
    * Fixed a problem with incorrect language loading with duplicate "elearn.js" in link
    * Positioning of "Share" QR Code is now anchored to the top of the window.
    Will work better in long iframes
    * Zoom containers of image galleries will be placed anchored to their
    corresponding gallery
* __1.0.6__:
  * Fixes:
    * Fixed a problem with the back-button not being displayed
    * Fixed a problem with overview of style `Kachel` not being displayed
    correctly in webkit browsers
* __1.0.5__:
  * New:
    * Image Slider descriptions can include HTML elements and are no longer only
    text based
    * Localization languages are loaded asynchronously
* __1.0.4__:
  * New:
    * CSS -> SASS/SCSS: use variables for color styling
    * Changed a few colors
    * Support for localized tabbed boxes with `lang-code-tab` instead of name
  * Fixes:
    * Undefined `lang-code`s will not overwrite element texts
    * Resize correctly after language change
    * Gallery image zoom will be displayed and resized correctly
* __1.0.3__:
  * New:
    * Support for localization including German and English language
    with `<.. lang="en">` or `eLearnJS.setLanguage("en")`
      * German is selected per default

_Hint:_ Extensions for _elearn.js_ were moved to their own repositories.

#### Older versions (currently not available in _english_)

* __1.0.2__:
  * Fehlerbehebungen:
    * Schriftarten zusätzlich als _.ttf_ hinzugefügt
    * Fehlerbehebungen für CSS Flex Attribut (WebKit)
    * Tooltips werden auch bei schmalen Fenstern nicht mehr aus dem Bild
    geschoben
  * Anderes:
    * Das eLearn.js wurde grundlegend Refactored. Alle Funktionen müssen jetzt
    über das `eLearnJS` Objekt aufgerufen werden und sind nicht mehr global
    vorhanden
* __1.0.1__:
  * Neuerungen:
    * Markdown Template wurde angepasst für das `atom-elearnjs` package
    * MathJax Link erneuert
    * Druck Darstellung verbessert
  * Fehlerbehebungen:
    * Kachlübersicht wird auch in geschachtelter Form korrekt dargestellt
    * Das Event `ContentResize` wird auf dem window.parent nun bei allen
    Größenveränderungen korrekt gefeuert
* __1.0.0__:
  * Neuerungen:
    * Die Pfeile für die Section-Wechsel wurden neu positioniert und die
    klickbaren Bereiche umfassen nun die volle Fensterhöhe
    * Für Section-Wechsel, Berechnungen bei Fenstergrößenveränderungen,
    Touch-Maus-Wechsel, Tab-Wechsel (für Tabbed-Boxes) werden nun Events
    gesendet
      * alle Funktionen die Events senden sind mit _@event_ gekennzeichnet
      * alte _registerAfter..._ Funktionen werden weiterhin unterstützt, zählen
      aber als veraltet
  * Fehlerbehebungen:
    * Im Template wurde die MathJax-Verlinkung angepasst
* __0.9.9__:
  * Neuerungen:
    * Bildergalerien springen bei einem Loop nicht mehr, sondern behalten
    die Bewegungsrichtung bei
    * Stil der Kacheln im Inhaltsverzeichnis angepasst
    * Stil von Slider, Multiboxes und ausklappbaren Bereichen angepasst
  * Fehlerbehebungen:
    * Fehler der Bildergalerien behoben
    * Auswahl von Text durch mehrfaches Klicken auf bestimmte Buttons entfernt
* __0.9.8__:
  * Neuerungen:
    * Automatischer Übergang zwischen Touch- und Maussteuerung auch während
    der Nutzung
  * Fehlerbehebungen:
    * Darstellungsfehler bei einzelnen Icons behoben
    * Fehler in Touch- und Maussteuerungserkennung bei iOS behoben
    * Fehlerbehebungen im Template
* __0.9.7__:
  * Neuerungen:
    * Einzelne Sections werden automatisch in den Browserverlauf aufgenommen
  * Fehlerbehebungen:
    * Fehler der Darstellung von Bildergalerien wurde behoben
    * Fehler bei der Gestensteuerung zum Seitenwechsel wurde behoben
    * Fehler, welche zu nicht funktionsfähigen Multiboxes und
    Mouseover-Informationsblöcken führten, wurden behoben
* __0.9.6__:
  * Neuerungen:
    * Mouseover-Informationsblöcke wurden eingeführt
    * Sections können in Sub- und Subsubsections geschachtelt werden
  * Fehlerbehebungen:
    * Beim Wechsel von Sections werden auch eingebundene Audiodateien gestoppt
    * Berechnung der Breite der Navigationsleiste wieder korrekt (vorher zu
    kurz)
* __0.9.5__:
  * Neuerungen:
    * Gelesen-Haken in Kachelinhaltsverzeichnis per _.hide-read_ deaktivierbar
    * Pfeiltasten können zur Navigation gedrückt gehalten werden
    * Umstrukturierungen der Ordner
  * Fehlerbehebungen:
    * Navigationsleistenberechnung jetzt abhängig von beinhalteten Elementen
* __0.9.4__:
  * Neuerungen:
     * Multiboxes und ausklappbare Blöcke wurden eingeführt
* __0.9.3__:
  * Neuerungen:
    * Eine Section lässt sich durch ihren Namen öffnen per _showSection(NAME)_
* __0.9.2__:
  * Fehlerbehebungen:
    * Gestensteuerung zum Section-Wechsel verbessert
    * Bilder werden nicht zwangsläufig auf 100% gestreckt, sondern bekommen dies
    als Maximalbreite
* __0.9.1__:
  * Neuerungen:
    * Überschrift einstellbar für den Fall, dass keine bestimmte Section sondern
    alle sichtbar sind per _eLearnJS.setNavigationTitle("Überschrift")_
    * Kachelübersicht
    * Man kann Funktionen registrieren, die ausgeführt werden sollen, nachdem
    eine andere Section angezeigt wird
    * Backbutton wurde eingeführt
    * Bestimmte Section per Parameter im Link aufrufbar
  * Fehlerbehebungen:
    * Ausklappbare Übersicht der Navigationsleiste wird nicht mehr falsch
    positioniert
* __0.9__:
  * Neuerungen:
    * Beschreibung für Kacheln im Inhaltsverzeichnis möglich
  * Fehlerbehebungen:
    * Kacheldarstellung für Microsoft Edge und Firefox angepasst
* __0.8__:
  * Neuerungen:
    * Kacheldarstellung für das Inhaltsverzeichnis
    * Einstellungsmöglichkeiten: Fortschrittsbalken, Richtungspfeile,
    Tastatursteuerung deaktivierbar
* __0.7__:
  * Neuerungen:
    * Inhaltsverzeichnis zur Einbindung in den Text verfügbar
    * Aktive Section wird in Inhaltsübersicht hervorgehoben
    * Automatische Erkennung der Downloadmöglichkeit der Seite als _EPUB_ oder
    _PDF_
    * Menü kann nur noch per Button geöffnet werden
    * Umbenennung einzelner Menüpunkte
    * Videos stoppen beim Section-Wechsel
    * Tooltip für Gestensteuerung zum Section-Wechsel
  * Fehlerbehebungen:
    * Die Inhaltsübersicht der Navigationsleiste ist scrollbar, wenn sie zu
    lang ist
    * isTouchSupported korrekt funktionsfähig
    * Ein Fehler bei der Tastatursteuerung wurde behoben
    * Performanceverbesserung durch weniger Größenberechnungen
    * Kein Section-Wechsel wenn Element vertikal gescrollt werden sollte
* __0.6__:
  * Statische Elemente nicht mehr in der HTML Datei sondern Fest im JavaScript
  * Tooltips für Grundelemente des eLearn.js
  * Fehlerbehebungen
    * Fehler mit Klicken auf Touch-Devices behoben
* __0.5__:
  * _Zu früheren Versionen sind keine Informationen mehr verfügbar_
