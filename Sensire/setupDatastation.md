# Opzetten datastation (triplestore)

Na installatie GraphDB, toevoegen jdbc drivers voor connectie MSSQL

In de grafische interface (GraphDB Workbench), linker menu - Help - System information. Ga naar tabblad Configuration Parameters. Onder de variabele graphdb.dist vind je de locatie waar de drivers neergezet moeten worden en waar de configuratie moet worden aangepast.
Voorbeeld OSX: /Applications/GraphDB Free.app/Contents/Java
Voorbeeld Linux: /opt/graphdb-free/app

Voor het gemak noem ik deze map even $Java

Plaats de juiste jdbc driver(s) in de map $Java/bin

Open 'GraphDB Free.cfg' en voeg de toegevoegde drivers uit de vorige stap toe aan het Classpath. Dit lijkt niet nodig te zijn bij installaties op een Windows platform.

Herstart GraphDB

Bij het aanmaken van een nieuwe "Ontop Virtual" repository krijg je bij de drivers nu ook de keuze MS SQL.