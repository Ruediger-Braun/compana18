=================================
Installation auf Windows-Rechnern
=================================

* Miniconda von der `Download-Seite`_ herunterladen.  Wählen Sie die Version  mit Python 3.7 für Ihr Betriebbsystem

* Die heruntergeladene Datei ausführen.  Dadurch startet das Installationsprogramm.  Am besten akzeptiert man alle Voreinstellungen.

* Öffnen Sie eine "Eingabeaufforderung" (finden Sie über die Suchfunktion) und installieren Sie die benötigten Bibliotheken mit dem Befehl 

.. code:: PowerShell

  conda install jupyter
  conda install scipy
  conda install sympy
  conda install matplotlib
  conda install scikit-image

Es ist im Prinzip möglich, alle fünf Installationen in einem Befehl 
durchzuführen; dann besteht allerdings die Gefahr, dass sich das 
Installationsprogramm bei der Berechnung des Abhängigkeitsgraphen 
aufhängt.
  
===================
Start des Notebooks
===================

Die graphische Oberfläche wird vom "Jupyter Notebook" zur Verfügung gestellt.  Man findet es über die Suchfunktion.

Wenn man das Notebook startet, sieht man zuerst eine Eingabeaufforderung.  Nach kurzer Wartezeit öffnet sich dann der Browser mit der lokalen jupyter-Seite.  





.. _Download-Seite: http://conda.pydata.org/miniconda.html




Fragen
======

* Wie bekommt man heraus, ob man 32-bit oder 64-bit Windows hat?

  Eine Antwort gibt `diese Seite von Microsoft`_





.. _diese Seite von Microsoft: https://support.microsoft.com/de-de/kb/827218
