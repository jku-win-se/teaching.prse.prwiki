

# Build Management with Maven

Maven ist ein Build-Management-Tool der Apache Software Foundation und basiert auf Java. Mit ihm kann man insbesondere Java-Programme standardisiert erstellen und verwalten. Entwicklungsumgebungen wie InteliJ und Eclipse besitzen Maven schon bei nach der Installation. Maven Projekte können direkt erstellt unter new Project usw.

Eine Standard Verzeichnisstruktur von Maven sieht folgendermaßen aus:


    src: alle Eingabedateien
        src/main: Eingabedateien für die Erstellung des eigentlichen Produkts
            src/main/java: Java-Quelltext
            src/main/resources: andere Dateien, die für die Übersetzung oder zur Laufzeit benötigt werden, beispielsweise Java-Properties-Dateien
        src/test: Eingabedateien, die für automatisierte Testläufe benötigt werden
            src/test/java: JUnit-Testfälle für automatisierte Tests
    target: alle erzeugten Dateien
        target/classes: kompilierte Java-Klassen

In Maven spielt die pom.xml eine wichtige Rolle, dort werden alle Softwareabhängigkeiten angegeben. Hierbei wird ermittelt, ob Maven die benötigten Dateien im lokal Repository vorhanden ist, falls dies der Fall ist wird beim Kompilieren die lokale Datei verwendet und nicht in das Projektverzeichnis kopiert.
Falls die Datei nicht im Repository vorhanden ist, versucht Maven über das Repository im Intranet oder Internet sich zu verbinden und die gewünschten Dateien in das lokale Repository zu kopieren.
Bekannte und öffentliche Maven Repositorys: Apache, Ibiblio, Codehaus oder Java.net
