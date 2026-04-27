In smarten Sensorsystemen werden Chips (inkl. Prozessor und Firmware) mit einem oder mehreren Sensorelementen zu einem Gesamtsystem integriert. 
Der Mehrwert entsteht dabei durch die komplexe Interaktion und Integration des Chips mit weiteren elektrischen und mechanischen Elementen (MEMS - Micro-Electro-Mechanical Systems).
Nur durch eine frühzeitige und ganzheitliche Berücksichtigung aller Komponenten kann ein erfolgreiches Gesamtsystem in der geforderten Time-to-Market mit niedrigsten Entwicklungskosten geliefert werden. 
Zur Optimierung der Chipfunktion in schnellen Iterationszyklen ist ein virtueller Prototyp erforderlich, d.h. ein Simulationsmodell des Gesamtsystems auf Systemebene, typischerweise in SystemC (standardisierte C++ basierende Systembeschreibungssprache). 
Um analoge Schaltungen und Sensorelemente (MEMS) in virtuellen Prototypen abzubilden, wird die ebenfalls standardisierte Analogerweiterung SystemC AMS genutzt. 
Die Beschreibungen der analogen Komponenten werden auf Differentialgleichungssysteme abgebildet. 
Die resultierenden Gleichungssysteme physikalischer Komponenten wie z.B. des mechanischen Teils von MEMS stellen spezielle anwendungsabhängige Ansprüche an den Gleichungslöser und die Zeitschrittweitensteuerung um korrekte Lösungen in akzeptabler Zeit zu berechnen.  
Die Projektpartner Bosch Sensortec und Universität Rostock haben bereits gemeinsam zur Gleichungslösung und dynamischer Schrittweitenanpassung bei der Simulation von MEMS geforscht und wichtige Grundlagen gelegt. 
Im Projekt wird eine Schnittstelle für SystemC AMS definiert, in den Standardisierungsprozess eingebracht und in die Open Source Referenzimplementierung integriert, die es erlaubt anwendungsspezifische Algorithmen zur Gleichungsaufstellung, -lösung und Zeitschrittweitensteuerung zu integrieren. 
Basierend auf dieser Schnittstelle und den Vorarbeiten von Bosch Sensortec und der Universität Rostock wird eine für die Modellierung von MEMS optimierte SystemC AMS Erweiterung als OSS Bibliothek entwickelt. 
Um eine breite Nutzung zu fördern und die Leistungsfähigkeit zu demonstrieren, wird zudem das Systemmodell eines smarten Sensors als Open Source zur Verfügung gestellt, um damit die bestehende Lücke der Erstellung virtueller Prototypen mit physikalischen Komponenten wie z.B. MEMS zu schließen.

IP-Blöcke, die häufig auch zu Projektbeginn bereits als eine Register Transfer Level (RTL) Beschreibung vorliegen, werden idealerweise direkt in den virtuellen Prototypen eingebunden.
Damit wird signifikant Aufwand für die explizite Modellierung und Verifikation dieser Blöcke eingespart.
Von IP-Blöcken, die parallel zum Sensorprojekt entwickelt werden, wird nach Projektbeginn eine abstrakte Beschreibung entwickelt.
Können wichtige IP Blöcke durch die RTL Beschreibung ersetzt werden, wenn diese vorliegt, wird ein besserer Kompromiss zwischen Simulationsgeschwindigkeit und Modellgenauigkeit des HVP ermöglicht und das Risiko für zeitaufwändige und kostspielige Iterationen für das Smartsensorprojekt reduziert.
Für die Hardwarebeschreibungssprache Verilog steht mit Verilator [VER25] ein leistungsfähiges und erfolgreiches OSS-Werkzeug zur Verfügung. In Europa ist jedoch VHDL die weitaus gebräuchlichere Sprache.
Diese Lücke im Open Source EDA-Tooling zum Nachteil europäischer Wettbewerber wird im Projekt HYPRSENSE adressiert und geschlossen. 
Dazu wird ein Tool entworfen und realisiert, das synthetisierbaren VHDL-Code einliest und vergleichbar zu Verilator ein SystemC Modul erzeugt.
Obwohl die in HYPRSENSE entstehende Open Source Software (OSS) durch Lückenschlüsse für die Entwicklung von Smart Sensor Systemen motiviert ist, werden die entwickelten Ansätze Wirkung über diesen Anwendungsbereich hinaus entfalten. 
Die Performance-Verbesserungen in SystemC AMS werden in allen Systemen sichtbar sein, deren Dynamik variiert. 
Verilator ist heute schätzungsweise auf vielen tausenden Systemen installiert, es wird vermutet, dass die VHDL-Unterstützung eine ähnlich große Verbreitung findet.