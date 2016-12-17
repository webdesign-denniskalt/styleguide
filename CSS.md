#CSS-Styleguide
===============

##Meine Denkweise
---------------
> Jede Zeile Code sollte so aussehen, als wäre sie von ein und derselben Person geschrieben. 

##Inhaltverzeichnis
-----------------
1. [Ordnerstruktur](#folderstructure)


##<a name="folderstructure">Ordnerstruktur</a>
----------------------------------------------
Eine gute Struktur ist für den gesamten Entwicklungsprozess wichtig. Daher sollte darauf geachtet werden, dass in jedem Projekt die selbe Basis gewährleistet wird. Das wird allen beteiligten Personen helfen. Das ist meine persönliche Struktur (nach [SMACSS](https://smacss.com/)):

```
scss/
|- _base/               # Standardelemente
|  |- _config.scss
|  |- _presets.scss
|  |- _headings.scss

|- _layouts/            # Bereiche
|  |- _l-base.scss
|  |- _l-grid.scss

|- _modules/            # Wiedernutzbare modulare Teile
|  |- _m-buttons.scss
|  |- _m-tabs.scss

|- _states/             # Aussehen in bestimmten Zuständen
|  |- _s-buttons.scss
|  |- _s-tabs.scss
|- _application.scss

layout/                 # Aussehen vom Layout
|- layout.css
```

##<a name="selector-depth">Tiefe von Selektoren</a>
---------------------------------------------------
Lediglich für :hover & :focus-Elemente sollten Selektoren eine Tiefe von 3 überschreiten. Denn je tiefer man selektiert, desto mehr Probleme treten im weiteren Entwicklungsprozess auf. Es sollte stets probiert werden, etwas mit weniger Selektoren auszuweisen.
