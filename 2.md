# Was stellt der Betrieb her?
Die Firma KDAB(Klarälvdalens Datakonsult AB) stellt Software her. Diese Software wird in speziellen Geräten und Desktop Computer eingesetzt.
Die Industrien für Geräte Software sind: Automobilindeustrie, Lebensmittelindustrie, Spieleindustrie, Medizintechnik, Metalindustrie, Luftfahrtindustrie

# Wie viele Leute arbeiten im Betrieb und was machen sie?
Ungefähr 100 Personen werden bei KDAB beschäftigt. Die Personen kommen aus über 20 Ländern, dies hat zur Folge,
dass die Firmen-Sprache Englisch ist. Ungefähr 70 Personsn von den 100 Beschäftigten Personen sind Software
Entwickler. Ungefähr 10 von den verblibenden Entwicklern sind System Administratoren. Die verbleibenden
Beschäftigten arbeiten in der Verwaltung und in Marketing Bereich.

# Wie lange gibt es den Betieb bereits?
Die Firma KDAB wurde am 11ten November 1999 gegründet von Kalle Dahlheimer. Kalle Dahlheimer war ein wichtiger KDE Entwickler zur der Zeit. KDAB arbeitete
am Anfang für Nokia und mit dem Sturz von Nokia konzentrierte sich die Firma auf andere Industrien um zu überleben. Die Firma KDAB hatte von der Gründung 
bis Heute circa über 600 Kunden gehabt.

# Was war heute meine Aufgabe ?
## Entwicklung
Die Aufgabe war es ein kleines Programm zu entwickeln, dass 3 grundlegende Funktionen der Speicher Verwaltung benutzt.
Nun sollte eine Bibliothek entwickelt werden, welches das kleine Programm manipuliert und die Speicherfunktionen ersetzt.
Auf der Platform Linux kann man das mit "LD PRELOAD" erreichen. "LD PRELOAD" ist eine Umgebungs-Variable die dem
Loader(so heißt das Program das Bibliotheken einbindet in Linux Programme) vorgibt eine Bibliothek vor allen anderen
Bibliotheken in das zu ausführende Programm einzubinden.

## Probleme
Eines der Probleme war gewesen dass eine Funktion sich selber aufgerufen hat was zur einer Endlosschleife geführt hat. Diese
Endlosschleife führte dann zur einem abrupten absturz des Programms.

## Lösung
Die Lösung war gewesen den Loader zu fragen wo die alte version der Funktion gewesen ist und die Addresse dieser Funktion zu Speichern und
diese Addresse vom Speicher aufzurufen in unserer eigenen Implementation der Speicher Verwaltungs Funktionen.

# Welches neuen Aufgaben nimmst du dir für Morgen vor?
Bisher musste die Bibliothek beim Start eines Programmes eingebunden werden vom Loader. Morgen nehme ich mir vor
mittels ptrace die Bibliotheks-Funktionen des Loaders in einem bereits laufendem Program auszuführen.
