# Produktivit�t als Programmierer
Da wir Programmierer l�sungs- und optimierungsorientierte Menschen sind befinden wir uns stetig auf der Suche nach einer M�glichkeit noch mehr aus uns herauszuholen. 
Aus einem Zitat von *Elon Musk* :
> "It's mostly about the bandwidth, the speed of the connection between your brain and the digital version of yourself, particularly output." 

wird klar dass viele Menschen sich mit diesen Problemen besch�ftigen.
Die [L�sung](https://de.wikipedia.org/wiki/Neuralink) die *Musk* anstrebt ist zwar noch 'Zukunftsmusik' aber wir k�nnen versuchen unseren Output zu steigern indem wir unsere Tools effizienter nutzen, nachfolgend werde ich auf verschiedene M�glichkeiten eingehen.

## Vim 
### Was ist Vim?
Vim ist ein Editor und stellt einen Clone des *vi*-Editors dar, der Name steht f�r "*Vi iMproved*".
Vim ist ein modaler Editor, d.h., der Editor unterscheidet zwischen verschiedenen Modi:
- *Normal*
- *Insert*
- *Visual*

Diese Modi gruppieren die verschiedenen Operationen.
#### Normal Mode
In diesem Modus wird durch das Dokument navigiert. Durch die ca. 700 Kommandos ist die Maus theoretisch nicht mehr von N�ten! Aber keine Angst du musst nicht alle beherrschen um klar zu kommen. Bereits mit einer kleinen Untergruppe der Befehle bist du in der Lage dich effizient durch ein Dokument zu bewegen. Unter [Vim Shortcuts](#vim-shortcuts) kannst du diese einsehen.

Anf�nglich ist ist es recht �berw�ltigend sich zurecht zu finden in der Vim-Welt, aber sie es als Investition! 
Schnell lernst du das du du keine Pfeiltasten ben�tigst um den Cursor zu navigieren, wir nutzen einfach <kbd>h</kbd><kbd>j</kbd><kbd>k</kbd><kbd>l</kbd>, verr�ckt oder?  Es ist auch m�glich nach Worten, S�tzen, Zeilen, Bildschirm- oder sogar Dokumentbereichen zu navigieren. So kannst du schnell ans Ende oder den Anfang einer Zeile Springen, du kannst Vim auffordern den Cursor im Bildschirm ganz oben, in der Mitte oder ganz Unten zu platzieren.
### Installation
Vim kannst du [hier](https://www.vim.org/download.php) herunterladen.

Wir werden au�erdem Vim als [Plugin](#vim-plugin) in *Eclipse* installieren und somit auch dort in den Genuss seiner Features kommen.
### Konfiguration
[TODO: vimrc]
#### Vim Shortcuts
Hier habe ich ein kleines [cheatsheet](./source/downloads/cheatsheet_vim.pdf) zusammen gestellt, dieses darfst du dir gerne herunterladen.

## IDE
### Eclipse
#### Vim-plugin
### Eclipse Shortcuts

## Tastatur
### Zehnfingersystem
Um den gr��tm�glichen Vorteil aus unseren m�chtigen Tools zu ziehen ist es von Vorteil nicht mehr auf die Tastatur sehen zu m�ssen und uns somit auf unsere Arbeit konzentrieren zu k�nnen! Da wir, dank [vim](#vim), nicht einmal mehr die Maus ben�tigen geschweige denn die Pfeiltasten k�nnen wir all unsere Arbeiten von der Grundstellung <kbd>a</kbd><kbd>s</kbd><kbd>d</kbd><kbd>f</kbd> und <kbd>j</kbd><kbd>k</kbd><kbd>l</kbd><kbd>�</kbd> aus erledigen! Wenn wir nun daran arbeiten sicher im [Zehnfingersystem](https://de.wikipedia.org/wiki/Zehnfingersystem) zu werden profitieren wir und unsere Arbeit von den Synergien die sich daraus ergeben!

Folgende Seiten empfehle ich hierf�r:
- [typingclub](https://www.typingclub.com/)
- [tipp10](https://online.tipp10.com/de)
- [typeracer](https://play.typeracer.com/)

### Tastatur-Layouts
Es gibt die verschiedensten Tastaturbelegungen, um einige zu nenen:

#### QWERTY
![qwerty](./source/images/QWERTY.png)
Diese Tastatur ist am weitesten verbreitet und wird im englischsprachigen Raum verwendet.

#### QWERTY
![qwerty](./source/images/QWERTZ_German.png)
Bild layout unser Layout das wir kennen und 'lieben?'.
Meiner Meinung nach ist diese Tastaturbelegung teilweise recht umst�nndlich zehnfingertippend zu programmieren. So ist zum Beispiel die geschweifte Klammer '{' recht umst�ndlich �ber <kbd>Alt Gr</kbd>+<kbd>7</kbd> oder �ber <kbd>strg</kbd><kbd>alt</kbd>+<kbd>7</kbd> zu tippen.

#### Colemak
![colemak](./source/images/Colemak.png)
Ist optimiert auf moderne Bed�rfnisse und eignet sich besonders f�r g�ngige Tastenk�rzel. Die Lage der Grundstellung wurde so gew�hlt um h�ufige Phrasen schneller tippen zu k�nnen.

#### Dvorak
![dvorak](./source/images/Dvorak.png)
Soll besonders ergonomisch sein und eignet sich besonders zum Programmieren!
Solltest du dich entscheiden *dvorak* einen Versuch zu widmen kannst du dies ebenfalls bei [typingclub](https://www.typingclub.com/dvorak) tun!

## Sonstige Software
### Autohotkey
Solltest dein [Tastatur Layout](#tastatur-layouts) nicht anpassen wollen oder du traust dich noch nicht diesen Schritt zu gehen dann kannst du die Belegung deiner Tastatur auch umgehen mit Tools wie *Autohotkey*. Ich habe hier die Navigation von Vim implementiert und lege die Belegung der geschweiften und eckigen Klammern um. 

#### Installation
Lade dir [AutoHotkey](https://autohotkey.com/) herunter.
Anschlie�end erstellst du ein `autohotkey.ahk`-Skript. 

#### Skripte
*AutoHotkey* kommt mit einer eigenen m�chtigen Skriptsprache diese wird interpretiert und erm�glicht Vielerlei!

Mein Skript sieht wie folgt aus:
```script
!h::Send,{Left}
!l::Send,{Right}
!k::Send,{Up}
!j::Send,{Down}
!b::Send,{[}
!n::Send,{]}
!v::Send,{{}
!m::Send,{}}
```
AutoHotkey kann noch viel mehr, ich nutze derzeitig aber nur dieses Feature.
[Hier](https://autohotkey.com/docs/Scripts.htm) findest du weitere Informationen.




