---
ID: 325
post_title: Untersuchung
author: rogera
post_date: 2010-09-21 18:13:42
post_excerpt: ""
layout: page
permalink: >
  http://wp.wolfspool.chickenkiller.com/wprcs1/pg-meta-pages/pg-sohorouter/untersuchung/
published: true
sharing_disabled:
  - "1"
---
<h2><strong>SOHO router exploitability analysis, malware for routers</strong></h2>
<strong><a href="mailto:sohorouter@gmail.com">sohorouter@gmail.com</a>, <a href="http://sohorouter.wordpress.com/">http://sohorouter.wordpress.com</a></strong>

Gefoerdert durch netidee 2008 (<a href="http://de.wikipedia.org/wiki/Netidee">http://de.wikipedia.org/wiki/Netidee</a>)
<h2><strong>Vorgehen</strong></h2>
Aus einem frei verfuegbaren Datenbestand der national zuordenbaren IP-Adressen wurden die ca 1.600 oesterreichischen IP-Bloecke entnommen. Von den 84 Eintraegen ueber 64k Adressen wurden alle mit mehr als 256k Adressen sowie einige kleinere Bloecke bearbeitet (insgesamt 16 Bloecke). Von den ca 11 Millionen Adressen sind dadurch etwa 3 Millionen Adressen betroffen. Leichte Abweichungen der nationalen Zuordnung im Vergleich mit anderen Quellen sind vernachlaessigbar. Einzelne Bloecke wurden nach Stichprobe als wenig ergiebig identifiziert, so ist beispielsweise ein gesamter Block offenbar nur fuer die Einwahl/Anbindung von mobilen Endgeraeten angelegt. Nachdem diese Zuordnung die Ergebnisse regional nach unten relativiert wurde darauf weiter keine Ruecksicht genommen - ein Gesamtscan, auch weltweit, wuerde diese Bloecke ebenfalls enthalten. Die teilweise von den tatsaechlichen Verhaeltnissen abweichenden Daten der geographischen Zuordnung beeinflussen die Aussage der Ergebnisse nicht und blieben unberuecksichtigt.

Ueber diese IP Adressen wurde ein zweistufiges Verfahren ausgefuehrt. Im ersten Schritt (SCAN) wurden mittels TCP-Scan auf jene Adressen reduziert, welche auf den Ports 80 und 8080 Services anbieten. Von diesen Systemen wurden die Resultate gezogen und nach Basic-Authentication Realms gefiltert. Die erhaltenen Realm-Bezeichnungen wurden gruppiert und fuer die weitere Betrachtung nur die Top 20 Treffer herangezogen. Gaengige Ports, die standardmaessig von einzelnen Routermodellen fuer den Fernwartungszugang verwendet werden, wie 88 oder 1080, wurden vernachlaessigt.

Die durch den ersten Schritt erhaltenen Realms wurden nach Routermodellen unterteilt. Jene Modelle, fuer die vom Hersteller Quellcode fuer die Firmware verfuegbar ist, und deren Firmware auch ueber die Remote-Administrations Anwendung geladen werden kann, wurden in einem zweiten Test (LOGIN) darauf geprueft ob mittels bekannter Standardeinstellungen Zugang gegeben ist.

Die Testserien wurden durchwegs in der Nacht abgesetzt, an den untersuchten Systemen wurden keinerlei Veraenderungen der Software oder von Einstellungen vorgenommen. Abgesehen von standardisierten Antworten der getesteten Geraete unmittelbar nach Anmeldung wurden keinerlei anschlussspezifische Daten entnommen, aufgezeichnet oder ausgewertet. Saemtliche Detailaufzeichnungen sind zu reinen Auswertungszwecken verfuegbar, wurden vollstaendig einer Versionskontrolle unterworfen, und werden nicht veroeffentlicht. Saemtliche Modifikationsprozesse fanden auf Laborgeraeten statt, welche in einem abgetrennten Netzwerk installiert waren. Die fuer die Testserien eingesetzte Software ist oeffentlich zugaenglich, neu erstellte Software ist publiziert und frei.

Die beiden Testvorgaenge fanden verschachtelt und zeitlich versetzt statt, wobei zwei Ergebnisschnitte vorliegen: MSRMT-1, MSRMT-2. Die Kennzahlen aus MSRMT-1 wurden fuer Auswahl zusaetzlicher manueller Erkundungen herangezogen. Zusaetzlich wurden geringfuegige Adressbereiche mit einer speziellen Realm-Suchmaschine sowie mittels Suche nach bestimmten Mustern via Google, Forenspam, Wikispam und Stichproben aus Blacklists herangezogen und die Trefferproportionen mit kleinen Stichproben von LOGIN-Tests verglichen, um einerseits das Kosten-Nutzenverhaeltnis des Scan Aufwandes festzustellen, andererseits um eventuelle Spuren von derzeit in Missbrauch stehenden Routern zu eruieren. Der geringe Anteil der Messergebnisse an den Gesamtzahlen wurde vernachlaessigt.
<h2>Messungen und Ergebnisrechnung</h2>
Aufgrund der demographischen Aehnlichkeiten von Oesterreich, Deutschland und Schweiz wurden die oesterreichischen Ergebnisse auf schaetzbare Verhaeltnisse im deutschsprachigen Raum extrapoliert. In einer zusaetzlichen Hochrechnung wurden die Resultate auf das gesamte Internet angewandt, wobei die damit erhaeltlichen Dimensionen natuerlich mit Einschraenkungen zu interpretieren sind. Als weiterer Umstand ist vorauszusetzen, dass grosse IP-Adressbloecke nicht notwendigerweise mit hoher Systemdichte korrelieren muessen, diese Einschraenkung aufgrund groesserer leerer Adresssegmente jedoch die Ergebnisse eher nach unten relativiert und deshalb vernachlaessigt wurde.

Das Verhaeltnis D/A/CH nach Adressumfang betraegt in etwa 10/1/2, fuer eine Extrapolation von oesterreichischen Ergebnisse auf den deutschsprachigen Raum wird somit ein Faktor von 13 angesetzt. Dies entspricht auch grob dem Bevoelkerungsverhaeltnis.
<table border="0" rules="NONE" cellspacing="0">
<tbody>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" width="365" height="17"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="LEFT" bgcolor="#E6E6FF" width="119"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="LEFT" bgcolor="#E6E6FF" width="67"><strong><span style="font-family: 'Andale Mono';">Factor</span></strong></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">DE</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">109,859,561</span></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">AT</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">11,156,240</span></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><strong><span style="font-family: 'Andale Mono';">Factor</span></strong></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">9.8473644346</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">10</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">CH</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">21,258,470</span></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">AT</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">11,156,240</span></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><strong><span style="font-family: 'Andale Mono';">Factor</span></strong></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">1.9055228285</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">2</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><strong><span style="font-family: 'Andale Mono';">Factor D/A/CH → AT*13</span></strong></td>
<td align="LEFT" bgcolor="#E6E6FF"></td>
<td align="RIGHT" bgcolor="#E6E6FF"><strong><span style="font-family: 'Andale Mono';">13</span></strong>

&nbsp;</td>
</tr>
</tbody>
</table>
Von den oesterreichischen Adressen wurden insgesamt ca 1/3 untersucht.
<table border="0" rules="NONE" cellspacing="0">
<tbody>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" width="365" height="17"><strong><span style="font-family: 'Andale Mono';">Processing AT</span></strong></td>
<td align="LEFT" bgcolor="#E6E6FF" width="119"><span style="font-family: 'Andale Mono';">
</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">Scanned</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">3,150,593</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">Unscanned</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">8,009,742</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">Sum</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">11,160,335</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">Scanned AT / Unscanned AT : s/u</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">0.39</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">Extrapolation Full Scan AT: u/s</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">2.54</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">Stretch = Extrapolation * Factor D/A/CH</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">33.05</span></td>
</tr>
</tbody>
</table>
Das Verhaeltnis nach IP-Adressraum zwischen AT, D/A/CH und WORLD. Beim weltweiten Adressraum wurden jene Laender abgeschnitten, deren Adressraum geringer als 1 Million ist.
<table border="0" rules="NONE" cellspacing="0">
<tbody>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" width="365" height="17"><strong><span style="font-family: 'Andale Mono';">Sum World</span></strong></td>
<td align="RIGHT" bgcolor="#E6E6FF" width="119"><span style="font-family: 'Andale Mono';">3,184,381,797</span></td>
<td align="LEFT" bgcolor="#E6E6FF" width="67"><span style="font-family: 'Andale Mono';">
</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">Sum &gt; 1m</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">3,160,249,441</span></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">Factor rel AT</span></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><strong><span style="font-family: 'Andale Mono';">283.27</span></strong></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">Factor &gt;1m rel D/A/CH</span></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><strong><span style="font-family: 'Andale Mono';">21.79</span></strong></td>
</tr>
</tbody>
</table>
Die Messung ergab ca 700 offene Router bei ca 6500 Systemen, fuer die eine Anmeldung erforderlich war. In einzelnen Faellen, bzw bestimmten Routertypen ist mit Standardeinstellungen keine Anmeldung erforderlich. Nachdem dies vor allem sehr alte Modelle betrifft, fuer die auch nur eine eingeschraenkte Verwertbarkeit besteht, wurden diese Systeme nicht weiter betrachtet.

Auf den deutschsprachigen Raum bezogen kann von ca 220.000 Systemen ausgegangen werden, fuer welche eine Anmeldung erforderlich waere, wovon ca 23.000 Router mit Standardeinstellung betrieben werden.
<table border="0" rules="NONE" cellspacing="0">
<tbody>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" width="365" height="17"><strong><span style="font-family: 'Andale Mono';">Ipscan-alive ports 80,8080 MSRMNT 2</span></strong></td>
<td align="RIGHT" bgcolor="#E6E6FF" width="119"><span style="font-family: 'Andale Mono';">34579</span></td>
<td align="LEFT" bgcolor="#E6E6FF" width="67"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="LEFT" bgcolor="#E6E6FF" width="30"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="LEFT" bgcolor="#E6E6FF" width="483"><span style="font-family: 'Andale Mono';">
</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">Realms (without unprotected systems)</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">6585</span></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="LEFT" bgcolor="#E6E6FF"></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">not all realms are routers, but some are even unprotected</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">Default Account ACK</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">842</span></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="LEFT" bgcolor="#E6E6FF"></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">Default User ACK only</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">144</span></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="LEFT" bgcolor="#E6E6FF"></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">(separate DI-524 check)</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">Default Admin ACK </span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><strong><span style="font-family: 'Andale Mono';">698</span></strong></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="LEFT" bgcolor="#E6E6FF"></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">Open Routers Default Admin D/A/CH found</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="LEFT" bgcolor="#E6E6FF"></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">Realms*Stretch</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">217,633.30</span></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="LEFT" bgcolor="#E6E6FF"></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">Admin*Stretch</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">23,068.80</span></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="LEFT" bgcolor="#E6E6FF"></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">Open Routers Default Admin D/A/CH expected</span></td>
</tr>
</tbody>
</table>
Im ersten Messungsschnitt wurde das Verhaeltnis der Gesamtzahlen zu 'low hanging fruit' ermittelt. Es ist erkennbar, dass etwas mehr als die Haelfte der erreichbaren Systeme auf die top 20 Routermodelle entfaellt, wovon wiederum circa 1/3 jene Modelle sehr leicht von aussen modifizierbar sind. In Summe kann davon ausgegangen werden, dass circa 1/5 aller rueckmeldenden Router extrem gefaehrdet sind, uebernommen zu werden. Diese Systeme bieten vor allem keinen oder nur geringen Schutz gegen Brute-Force Attacken, teilweise wuerden solche Versuche nicht in einem Systemlog sichtbar.
<table border="0" rules="NONE" cellspacing="0">
<tbody>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" width="365" height="17"><strong><span style="font-family: 'Andale Mono';">Manual analytics MSRMNT 1 (slightly less data)</span></strong></td>
<td align="LEFT" bgcolor="#E6E6FF" width="119"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="LEFT" bgcolor="#E6E6FF" width="67"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="LEFT" bgcolor="#E6E6FF" width="30"></td>
<td align="LEFT" bgcolor="#E6E6FF" width="483"><span style="font-family: 'Andale Mono';">
</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">complete realms</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">5,184.00</span></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="LEFT" bgcolor="#E6E6FF"></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">Top-20</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">2,837.00</span></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="LEFT" bgcolor="#E6E6FF"></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">Factor</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">0.5472608025</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><strong><span style="font-family: 'Andale Mono';">0.5</span></strong></td>
<td align="LEFT" bgcolor="#E6E6FF"></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">½ of router models are mainstream models</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="LEFT" bgcolor="#E6E6FF"></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">Difficult Realms</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">2,093.00</span></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="LEFT" bgcolor="#E6E6FF"></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">Easy Realms</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">744.00</span></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="LEFT" bgcolor="#E6E6FF"></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">Factor</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">0.3554706163</span></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="LEFT" bgcolor="#E6E6FF"></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">1/3 of router models with easy to build custom firmware</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="LEFT" bgcolor="#E6E6FF"></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">Weight Top20: Realms/Easy</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">0.1945351348</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><strong><span style="font-family: 'Andale Mono';">0.2</span></strong></td>
<td align="LEFT" bgcolor="#E6E6FF"></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">1/5 of open routers are easy to take, modify firmware</span></td>
</tr>
</tbody>
</table>
Eine Einteilung von erreichten Systemen nach Realm zeigt, dass auf die Top 20 von ca 1100 verschiedenen Rueckmeldungstexten etwa 50% der Einheiten entfallen, und diese als Mainstream-Modelle anzusehen sind. Der folgende Datenblock zeigt die Verteilung und das Verhaeltniss zwischen nachweislich kontrollierbaren Systemen und jenen, fuer die eine Uebernahme mit groesseren Komplikationen verbunden ist. Die Moeglichkeit, eine open-source Firmware aufzubringen, wird dabei ausdruecklich nicht beruecksichtigt.
<pre><span style="font-family: Georgia, 'Times New Roman', 'Bitstream Charter', Times, serif; line-height: 19px; white-space: normal; font-size: 13px;">[Liste mit ca 1100 Eintraegen, davon ein grosser Block mit SpeedTouch-MAC Signatur]</span></pre>
<table border="0" rules="NONE" cellspacing="0">
<tbody>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" width="309" height="17"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="LEFT" bgcolor="#E6E6FF" width="49"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="LEFT" bgcolor="#E6E6FF" width="45"><span style="font-family: 'Andale Mono';">easy</span></td>
<td align="LEFT" bgcolor="#E6E6FF" width="86"><span style="font-family: 'Andale Mono';">difficult</span></td>
<td align="LEFT" bgcolor="#E6E6FF" width="61"><span style="font-family: 'Andale Mono';">Top 20</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><strong><span style="font-family: 'Andale Mono';">Total Result</span></strong></td>
<td align="RIGHT" bgcolor="#E6E6FF"><strong><span style="font-family: 'Andale Mono';">5184</span></strong></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">744</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">2093</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">2837</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">dreambox</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">599</span></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">599</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">599</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">WRT54GL</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">288</span></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">288</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">288</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">Thomson</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">282</span></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">282</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">282</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">Broadband Router</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">221</span></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">221</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">221</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">WGR614v7</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">188</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">188</span></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">188</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">NETGEAR WGR614v9</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">162</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">162</span></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">162</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">SpeedTouch</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">153</span></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">153</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">153</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">Login to the Router Web Configurator</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">151</span></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">151</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">151</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">WRT54G</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">125</span></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">125</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">125</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">WGR614v6</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">102</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">102</span></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">102</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">RP614v4</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">101</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">101</span></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">101</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">WGT624</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">70</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">70</span></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">70</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">NETGEAR WNDR3700</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">68</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">68</span></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">68</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">level_15_access</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">55</span></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">55</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">55</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">DI-524</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">53</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">53</span></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">53</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">WL-5460AP v2</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">49</span></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">49</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">49</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">WPN824v2</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">47</span></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">47</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">47</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">WRT54GS</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">47</span></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">47</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">47</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">Linksys BEFSR41</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">40</span></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">40</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">40</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">DI-804HV</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">36</span></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">36</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">36</span></td>
</tr>
</tbody>
</table>
Hochrechnung auf den deutschsprachigen Raum und Gesamtverhaeltnis
<table border="0" rules="NONE" cellspacing="0">
<tbody>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" width="365" height="17"><strong><span style="font-family: 'Andale Mono';">Result Expectation D/A/CH</span></strong></td>
<td align="LEFT" bgcolor="#E6E6FF" width="119"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="LEFT" bgcolor="#E6E6FF" width="67"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="LEFT" bgcolor="#E6E6FF" width="30"></td>
<td align="LEFT" bgcolor="#E6E6FF" width="483"><span style="font-family: 'Andale Mono';">
</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">Realms easy brute-forceable</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">43,526.66</span></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
<td align="LEFT" bgcolor="#E6E6FF"></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">
</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">Easy Admin</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">4,613.76</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><strong><span style="font-family: 'Andale Mono';">0.1</span></strong></td>
<td align="LEFT" bgcolor="#E6E6FF"></td>
<td align="LEFT" bgcolor="#E6E6FF"><span style="font-family: 'Andale Mono';">1/10 of easy routers are open</span></td>
</tr>
</tbody>
</table>
<table border="0" rules="NONE" cellspacing="0">
<tbody>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" width="365" height="17"><strong><span style="font-family: 'Andale Mono';">Result Expectation</span></strong></td>
<td align="LEFT" bgcolor="#E6E6FF" width="119"><span style="font-family: 'Andale Mono';">
</span></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><strong><span style="font-family: 'Andale Mono';">Top Countries &gt; 1m Addresses</span></strong></td>
<td align="LEFT" bgcolor="#E6E6FF"></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">Realms easy brute-forceable</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><strong><span style="font-family: 'Andale Mono';">948,452.34</span></strong></td>
</tr>
<tr>
<td align="LEFT" bgcolor="#E6E6FF" height="17"><span style="font-family: 'Andale Mono';">Easy Open Admin</span></td>
<td align="RIGHT" bgcolor="#E6E6FF"><strong><span style="font-family: 'Andale Mono';">100,534.51</span></strong></td>
</tr>
</tbody>
</table>
<h2>Fazit</h2>
Die Untersuchung hat gezeigt, dass im deutschsprachigen Raum mit etwa 4.600 Routern zu rechnen ist, welche nicht nur mit Standardeinstellungen in Betrieb sind, sondern auch zusaetzlich ueber den WAN-seitigen Zugang vollstaendig kontrolliert oder modifiziert werden koennen und fuer die eine Firmware leicht herstellbar ist. Weiters sind etwa 44.000 Systeme hochgradig gefaehrdet, nach Ueberwindung des trivialen Sicherungsmechanismus unter Fremdkontrolle zu geraten. Bei Uebertragung des Ergebnisses auf weltweite Verhaeltnisse waere mit etwa 100.000 offenen und ca 1 Mio extrem gefaehrdeten Routern zu rechnen. Mit der zusaetzlichen Schwierigkeit, fuer einzelne Routermodelle eine Firmware zu erzeugen, welche vom Aussehen nicht als speziell erkennbar waere, gelten die dreifachen Zahlen. Bei Nutzung verfuegbarer Routerfunktionen ohne Modifikation der Firmware, beispielsweise zum Scannen des LAN-Segments durch DMZ-Eintraege oder Port-Forwarding, faellt diese Schwierigkeit weg.

Diese Schaetzung verhaelt sich stimmig zu publizierten Daten, welche [psyb0t: 80k-100k] und [vxWorks: 250k / 3.1 Mrd. Addressen] Bedrohungen dokumentieren. Der zusaetzliche Aufwand, Firmware in verschiedenen Sprachen und fuer weitaus mehr Firmware-Releases fertigen zu muessen, darf dabei aber nicht ausser acht gelassen werden.

Gesondert wurde festgestellt, dass von einigen Geraetemodellen Adresslisten erheblichen Ausmasses zu einem im Verhaeltnis zu erzielbaren Verwertungsmoeglichkeiten geringfuegigen Preis online erhaeltlich sind. Einzelne Tests haben gezeigt, dass diese Daten teilweise veraltet sind und eine Datenqualitaet von ca 50% erreichen, was in Anbetracht der Datenmenge allerdings nicht generalisiert wird. Auch sind nicht fuer alle SCAN-Treffer entsprechende Daten erhaeltlich. Dennoch wuerde ein Erwerb eine wesentliche Zeit- und Aufwandsersparnis bedeuten, insofern die wesentlich groessere SCAN-Stufe uebersprungen werden koennte, und selbst mit der Haelfte von verfuegbaren Datensaetzen sehr rasch eine groessere Ausbeute an Treffern erzielbar waere.

----

[psyb0t] http://www.dronebl.org/blog/8

[vxWorks] http://blog.metasploit.com/2010/08/vxworks-vulnerabilities.html