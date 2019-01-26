============================================================
Installation von Mayavi auf Linux-Systemen
============================================================

Voraussetzung ist, dass conda bereits installiert ist.  Mayavi besitzt viele
externe Abhängigkeiten, daher sind Probleme bei der Installation nicht selten.
Aus diesem Grund installiert man es besser in eine neue Umgebung, die wir
`mayavi` nennen.  Die nötigen Befehle sind

.. code:: bash
    
    conda create -n mayavi
    conda activate mayavi
    conda install -c conda-forge mayavi
    conda install -c conda-forge scipy sympy
    conda install -c conda-forge ipywidgets ipyevents

Anschließend installiert man die für das Notebook erforderlich Erweiterung und
schaltet sie ein

.. code:: bash

    jupyter nbextension install --py mayavi --user
    jupyter nbextension enable --py mayavi --user

Dann kann man die Beispiele aus der Dokumentation_ ausprobieren.  Wenn die
Bilder schlecht aussehen (z.B. unstetige Farbverläufe), dann kann das an
Problemen bei der Zusammenarbeit von `qt5` und `mayavi` liegen.  In diesem
Fall entfernt man die Umgebung und baut sie neu wie folgt auf:

.. code:: bash
    
    conda env remove -n mayavi
    conda create -n mayavi
    conda activate mayavi
    conda install python=3.6 pip
    conda install -c conda-forge qt=4 pyqt
    pip install scipy
    pip install mayavi
    pip install sympy
    pip install ipywidgets
    pip install ipyevents

Die Erweiterungen beiben registriert.

.. _Dokumentation: https://docs.enthought.com/mayavi/mayavi/mlab.html#a-demo

