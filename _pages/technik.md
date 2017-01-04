---
ID: 326
post_title: Technik
author: rogera
post_date: 2010-09-21 18:15:12
post_excerpt: ""
layout: page
permalink: >
  http://wp.wolfspool.chickenkiller.com/wprcs1/pg-meta-pages/pg-sohorouter/technik/
published: true
sharing_disabled:
  - "1"
---
<h2>Scan</h2>
Die abgelaufenen Abfragen gegen die IP-Adressen sind direkt erfolgt, mit 5-10 Abfragen pro Sekunde ist die Netzwerkbelastung minimal - d.h. man kann mit geringer bzw haushaltsueblicher Bandbreite zum Ergebnis gelangen. Die zu testenden Adressen wurden innerhalb ihres Blocks grob verwuerfelt. Netzwerktests, welche guenstigerweise mit wesentlich hoeheren Datenraten abzufuehren sind koennten bereits ueber die aus Stufe 1 'eroberten' Endpunkte geleistet werden. Nur zu Pruefzwecken wurden geringe Teile ueber gesichert anonyme Verbindung abgearbeitet. Die dadurch auftretende Latenz ist weitgehend vernachlaessigbar. Ein weiterfuehrender Scan eines LAN-Segments mittels DMZ-Eintrag wurde mit dem schwaechsten verfuegbaren Routermodell labormaessig geprueft. Es ist davon auszugehen, dass der Erfolg auf alle Router mit dieser Funktionalitaet uebertragbar ist. Ein weiterfuehrender Scan eines LAN-Segments mittels Port-Forwarding wurde mit mehreren Routermodellen mit ebensolchen Ergebnissen geprueft.
<h2><strong>Login</strong></h2>
Bei einzelnen Routermodellen erfolgt nach Anmeldung zur Administration eine Sperre fuer weitere Adressen. Im Falle eines Angriffs, welcher mittels TOR anonymisiert vorgenommen wuerde, kommt es dadurch nach Wechsel des TOR-Exitpoints zu einer Wartezeit, bis der Prozess fortgesetzt werden koennte. Durch geeignete Automationsschritte, welche leicht herstellbar sind, wuerde die Attacke mit zwischenzeitlichen Abmeldungen nur unwesentlich verzoegert. Vor allem aeltere Routermodelle sehen allerdings keine Abmeldefunktion vor. Die Gesamtmetrik der Messung wuerde sich dadurch allerdings nicht wesentlich verschieben.
<h2>Routerspezifische Anmerkungen</h2>
Die Firma Netgear stellt fuer die Firmware ihrer Routermodelle den Quelltext zum Download. Das erhaeltliche Paket ist nicht wie dokumentiert verwendbar, jedoch kann mit einem generellen Ueberblick ueber die Werkzeugkonfiguration zur Herstellung von angepasster Firmware eine funktionsfaehige Version erstellt werden. Die erhaeltlichen Quelltexte umfassen im allgemeinen die Vorgaengerversionen der aktuellen Firmware, welche mit den Modellen gegenwaertig ausgeliefertwird. Bei der Herstellung einer Firmware mit den erhaeltlichen Quellen wird allerdings eine Vermengung von vorgefertigten Komponenten mit GPL/open source Komponenten erzeugt. Fuer die vorgefertigten Teile, beispielsweise das System aus Webserver des Routers (httpd) sowie der konkreten Verwaltungsseiten, ist kein Quelltext verfuegbar. Die Anpassung von Firmware-Versionen an die Sprachausstattung erfolgt auf voellig undokumentierte Weise, und traegt insgesamt deutliche Spuren einer gewachsenen, vertrackten Werkzeuginfrastruktur. Ob dahinter lediglich der erreichte Fortschritt an Vereinheitlichung oder eine eventuelle Verschleierungsabsicht steht ist nicht eindeutig beantwortbar  - fuer beides sind Argumente denkbar. So ist beispielsweise bei einzelnen Modellen die Moeglichkeit zum Firmware-Update in der WAN-seitigen Administrationsoberflaeche lediglich ausgeblendet, laesst sich jedoch bei gezieltem Aufruf nuetzen. Dies ist ein typischer Fall von 'Security by Obscurity', und es ist davon auszugehen, dass eine deutliche Nachvollziehbarkeit im Quelltext der Firmware vor allem wegen der Imagewirkung beim erwartbar versierten Publikum unerwuenscht gewesen ist.

Bei mindestens einem Modell eines Belkin-Routers wird zum Zweck der Passwort-Verifikation ebenjenes mit an den Webbrowser gesendet und kann im Quelltext der Verwaltungsseite ausgelesen werden. Da dieses Modell in der stattgefundenen Untersuchung nicht aufgefunden wurde, und eine Suche der Signatur mit der spezialisierten Suchmaschine http://shodanhq.com nur eine geringe Anzahl an Treffern ausweist, besteht vermutlich keine Automationswuerdigkeit hinsichtlich der Nutzung dieser Sicherheitsluecke. Bei allen Routern neueren Ursprungs ist erkennbar, dass solcherart Luecken vermieden werden. Die eingegebenen Passworte werden verschluesselt uebertragen, und koennten nur im selben Netzsegment abgehoert werden. In jenen Faellen, in denen md5 zur Anwendung kommt ist es jedoch zwischenzeitlich praktikabel geworden, mit breit verfuegbaren Mitteln eine gezielte Dekodierung zu erreichen. Unter der wesentlich schwierigeren Voraussetzung, den Netzwerkverkehr in beliebigen Netzsegmenten aufzeichnen zu koennen [bgp1], koennte eine automatisierte Entschluesselung auf skalierbare Weise erzielt werden. Obwohl in diesem Fall die Verantwortung eindeutig den Service Provider betraefe, ist auch aus diesem Grund von der Verwendung von Remote-Admin abzusehen.

Die dokumentierte Moeglichkeit bei einigen aelteren Geraeten, als Port-Forward Ziel eine externe WAN-Adresse einzutragen, ist bei Modellen neuerer Bauart generell nicht mehr vorhanden. Es bleibt allerdings anzumerken, dass eine solche Funktion mit entsprechender Firmware dann leicht einzurichten ist, wenn die Pruefung auf gueltige Innenseiten-Adresse lediglich in der Administrationsoberflaeche des Routers durch Einschraenkung der Eingabewerte vorgenommen wird.

====

[.onion] fuer die Identifikation von TOR-traffic ist, so ueberhaupt moeglich, die Kontrolle ueber eine groessere Anzahl von Teilnehmer- oder Endpunkten mindestens erforderlich.

vgl <a href="http://oreilly.com/pub/wlg/7333">http://oreilly.com/pub/wlg/7333</a> (2005) und <a href="https://www.defcon.org/images/defcon-18/dc-18-presentations/D.Brown/DEFCON-18-Brown-TorCnC.pdf">https://www.defcon.org/images/defcon-18/dc-18-presentations/D.Brown/DEFCON-18-Brown-TorCnC.pdf</a> (2010)

[bgp1] <a href="http://www.wired.com/threatlevel/2008/08/revealed-the-in/">http://www.wired.com/threatlevel/2008/08/revealed-the-in/</a>