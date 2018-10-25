# Data Analytics Tutorial
Dieses Tutorial soll eine Einführung in die Arbeit eines Analysten auf Basis von Python bieten.

## Installation
Für das Tutorial wird Anaconda verwendet, das frei für Windows, Linux und MacOS herunterladen werden kann:
https://www.anaconda.com/download/

Dieses Tutorial sieht die Verwendung von CentOS vor, eine Abbildung auf Windows oder MacOS sollte jedoch trivial sein.

## Einrichten eines eigenen Enviroments
Nach der Installation von Anaconda wird ein eigenes Environment für das Tutorial eingerichtet. Das hat den
vorteil, dass der Analyst selbst bestimmen kann, welche Versionen er/sie von welcher Bibliothek verwendet
und welche Version von Python genutzt werden soll.

Es ist ratsam für ein Environment einen eigenen Ordner anzulegen auch wenn ein Environment keinen festen Bezug zu einer Ordnerstruktur im Filesystem hat (außer den Ordner in dem Metadaten für die jeweilige Umgebung abgelegt werden).

Durch das Klonen dieses Repositories wird automatisch ein Ordner angelegt.

'''
git clone https://github.com/padmalcom/datutorial
'''

Nun kann das Enviroment angelegt werden.

'''
conda create -n datutorial
'''

Der Name "datutorial" ist frei wählbar, jedoch erinnert man sich bei vielen Environments leichter an dessen Namen, wenn er den Namen des Ordners trägt, in dem die Daten für das entsprechende Environment liegen.

Die abschließende Frage ist mit "y" zu bestätigen. Folgend kann das Environment aktiviert werden:

'''
conda activate datutorial
'''

Wenn nun Python-Befehle ausgeführt werden, geschieht das immer im Context dieses Environments (zu sehen an dem Namen vor der Befehlszeile).

## Installation notwendiger Pakete über pip
Python verfügt über verschiedene Paketmanager, die die Installation von Bibliotheken ermöglichen. Der bekannteste ist pip. Dieser muss jedoch zuvor installiert werden.

'''
conda install pip
'''

Nachfragen sind per "y" zu bestätigen. Ist pip installiert, können folgend alle weitere Bibliotheken darüber installiert werden.

'''
pip install matplotlib
'''

Es gilt im Hinterkopf zu behalten, dass pip und matplotlib damit **nur** in diesem Environment (datutorial) zu verfügung stehen.

## (Optional): Deaktivieren eines Environments
Sollte in einem anderen Environment gearbeitet werden, kann das aktuelle über folgenden Befehl verlassen werden.

'''
conda deactivate
'''

## Installation von Jupyter Notebook
Das Jupyter Notebook ist eine Webanwendung, die die Aufgaben Entwicklung, Dokumentation und Reporting unterstützt. Um es für dieses Tutorial verwenden zu können, muss es zunächst installiert werden.

'''
pip install jupyter
'''

Nachfragen sind wie gehabt über "y" zu bestätigen.

Im Folgenden kann die Anwendung gestartet werden.

'''
jupyter notebook
'''

Sollet sich kein Browser-Fenster öffnen, ist der Link, der in der Console steht zu kopieren und manuell in den Browser einzufügen.

Achtung: Der Root-Pfad des Notebooks ist immer der, aus dem der Befehl 'jupyter notebook' ausgeführt wurde. Sollte nur der Root-User für den Start des Notebooks zu Verfügung stehen, ist der Befehl so zu verwenden 'jupyter notebook --allow-root'.
