# Creating a postcard with Scribus

## Creating the document

Create a new document with two pages of the size of the postcard.

- The margin is not relevant. generell, würde ich trotzdem ein .5 oder 1 cm rand definieren.
um sicher zu stellen, dass kein text zu nah am rand kommt... (oder
gleich weit kommt).

## Creating the "front" page

Auf der forderseite werden ein oder mehrere Bilder mit eventell ein Text hinzugefügt.

Falls um das Bild ein weisser rand geben soll, solltest du vermutlich dieser Rand für die Seite benutzen.

wenn das foto bis am rand kommen soll, soltest du unbeding ein
anschnitt (bleed) definieren.

Um das bild auf der seite grösse zu definieren:

- Wähle das bild-tool
- die "shift" (in deutschland "umschalt") taste beim klicken drucke, um ein
  bildrahmen zu definieren, der so gross ist wie die ränder.
- in der eigenschaftspalette
  - die x und y werte auf 0 setzten,
  - breite auf `pagewidth` und höhe auf `pageheight` setzen (pagewidth und pageheight
    werden von scribus erkannt und mit der breite und höhe der seite
    automatisch ersetzt) dann kriegst du ein bild, das so gross ist wie die
    seite.

Wenn du 2 mm anschnitt definiert hast, dann setzt du

- x: -2mm
- y: -2mm
- width: pagewidth + 4mm
- height: pageheight + 4mm

wievel anschnitt du brauchst, das musst du bei flyeralarm nachschauen.
ich konnte die spez auf der schnelle nicht finden.

## Fitting the image in the frame

wenn das foto nicht das gleiche format wie der seite hat, dann:

- in der eigenschaftspalette > image tab
- die skalierung auf "Scale to Frame Size" setzen (mein scribus spricht
  englisch, sorry)
- Proportional deaktivieren
- Auf "Free Scaling" wechseln
- auf der kette rechts von x-scale / y-scale clicken um die proprtionen
  zu behalten
- jetzt kannst du x-pos oder y-pos so ändern, dass bild gut im rahmen
  passt (auchtung: es dürfen keine weisse bänder geben!)

## Creating the back page

