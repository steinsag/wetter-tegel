# Explorative Datenanalyse mit Jupyter Notebooks

In diesem Repo spiele ich etwas mit Jupyter Notebooks, um verschiedene
Datensätze zu analysieren.

Jupyter Notebook direkt ausführen: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/steinsag/wetter-tegel/master?filepath=notebooks%2Fwetter.ipynb)

## Setup der Conda Umgebung

Die Jupyter Notebooks können zum Beispiel in einer Conda Umgebung ausgeführt
werden. Alle benötigten Abhängigkeiten sind in der scipy-p37 Conda Umgebung
enthalten, die in `environment.yml` beschrieben ist.

Eine neue Umgebung anhand dieser Beschreibung erstellt man:

    conda env create -f environment.yml

Diese Datei habe ich folgendermaßen erstellt:

    conda env export > environment.yml

Eine lokale Umgebung kann anhand der `environment.yml` Datei folgendermaßen
aktualisiert werden:

    conda env update --file environment.yml --prune

## Jupyter Notebook starten

Die gewünschte Conda Umgebung wird folgendermaßen aktiviert:

    conda activate scipy-p37

Danach kann man Jupyter Notebooks starten:

    jupyter notebook

Dies startet einen lokalen Jupyter Server. Im Browser wird die zugehörige Web
GUI geöffnet.

In der Conda Umgebung ist ebenfalls die neue Jupyter Labs Web GUI enthalten.
Diese kann statt der Notebook Oberfläche gestartet werden.

    jupyter lab
