# Streetdudes

A visual presentation of streets in Ulm named after women, and named after men.

## Background

This map was created as part of a [Codeweek.eu](http://codeweek.eu/) hackathon organized by the [datalove working group at Ulm University](http://www.ulmapi.de). Originally, the idea was to examine street names with colonial backgrounds dating back to times of the German Empire – but, to our pleasant surprise, Ulm has either not followed the “tradition” of other German cities of naming streets after colonies or colonizers, or got rid of problematic street names in the past.

However, browsing through the [street name catalogue](http://daten.ulm.de/daten/single/strassenverzeichnis-und-gewannnamen) provided in [the city's Open Data portal](http://daten.ulm.de/), we noticed a rather stark contrast as to the vast number of streets named after men, and the comparatively small number of streets with women as their name patrons. Thus, the idea of visualizing this discrepancy was born and put into practise.


## Technical Background

The basemap is made with the [ever-so-ubiquitous Leaflet,](http://leafletjs.com) using the tile server provided by [Berlin's OK Lab](http://codefor.de/berlin). The streets categorized as being named either after a man or a woman were then extracted from OpenStreetMap data in [QGIS](http://www.qgis.org) an each put into a seperate GeoJSON file, which are then superimposed on the basemap.


## Who was Wera, anyway?

Unfortunately, the city's street catalogue lacks information on streets' name (m/p)atrons, or when a street was named. Upon request, the city of Ulm's Open Data team was quick as always with a reply – pointing us to one of the many projects that [ZAWiW (Zentrum für allgemeine wissenschaftliche Weiterbildung)](http://uulm.de/?zawiw) at Ulm University had undertaken earlier – in this case, researching the female name-givers of streets in Ulm and Neu-Ulm.

ZAWiW promptly provided us with the result of this project: A book with in-depth stories about the women deemed notable enough to give their names to a street or plaza in Ulm. If you are interested and have a chance, please pick up this book (ISBN: 978-3-88294-404-4) and give it a read. We, for one, would never have thought that Werastraße was named after [Grand Duchess Vera Constantinovna of Russia, Duchess of Württemberg](https://en.wikipedia.org/wiki/Grand_Duchess_Vera_Constantinovna_of_Russia), and were fascinated by Mathilde Wieland, who led the [Wieland metal works](https://de.wikipedia.org/wiki/Wieland-Werke) for 14 years following her husband's death (Mathildenstraße in Ulm-Oststadt).

For the male name patrons, we could not find a similar list – therefore, there might be some streets we overlooked. However, this would make the discrepancy between male and female namegivers only even more pronounced.


## Shouldn't we rather name streets after, say, places, or your favorite cheese, or wines, instead of people?

We don't know. A rather long list of streets in Ulm is already named after geographical features, types of wines, etcetera, and we'd certainly love to see cheeses included in this list. As to whether persons should or shouldn't lend their names to streets, that's up to the reader. Our main interest lay in visualizing those streets – and, after we found out the stories behind the women in Ulm's street names, passing those on to the interested reader.

During the NS reign, quite a lot of streets were re-named from bearing the names of persons to those of “neutral” entitites or NS figures. For instance, Olgastraße (named after [Queen Olga of Württemberg](https://en.wikipedia.org/wiki/Olga_Nikolaevna_of_Russia)) became Adolf-Hitler-Ring, Albert-Einstein-Straße became Fichtestraße, and so on.

After Nazi Germany was defeated, many of the street renamings were rolled back. Albert Einstein, however, suggested to change the name “his” street to “Weathervane Road” – thus, the city could save on costs for re-naming the street, should the political winds change again…

> „Ich glaube, ein neutraler Name, zum Beispiel ,Windfahnenstraße‘, wäre dem politischen Wesen der Deutschen besser angepasst und benötigte keine Umtaufen im Laufe der Zeiten.“


## Contributors


### Codeweek.eu: UlmAPI Hackday Team

* Christoph Amann
* Sandro Eilert
* Jana Funke
* Stefan Kaufmann

### Arbeitskreis Frauengeschichte

Authors of `Eigenwillig und couragiert – Wegweisende Frauen in Ulm und Neu-Ulm`:

* Ursula Bischoff
* Erdmute Dietmann-Beckert
* Jutta Gotthardt
* Barbara Heinze
* Ulrike Iffland
* Monika van Koolwijk
* Brigitte Nguyen-Duong
* Dr. med. Erla Spatz-Zöllner
* Andrea Toll
* Agathe Wende
* Mona Willmann
* Dr. Uta Wittich

### Further support

* Lucia Erdt (Stadt Ulm)
* Markus Marquardt (ZAWiW, Ulm University)
* Klaus Urmetzer (Stadt Ulm)

### How to contribute

Send in pull requests. Especially if it improves the usability in any way.

## Changelog

### 2014-11-09

* ADDED: README.md

### 2014-11-10

* CHANGED: gals.geojson now includes a series of streets previously missing; including information on the name givers (yet to be included into the visualization)

### 2014-11-11

* CHANGED: dudes.geojson sanitized

### 2014-11-12

* CHANGED: index.html now shows information on the female namegivers
