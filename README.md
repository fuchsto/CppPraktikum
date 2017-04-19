
STL-konforme Algorithmen und Container als Python-Extensions

In Forschungsbereichen wie Scientific Computing und Machine Learning hat
sich Python im Laufe der letzten zehn Jahre als Programmiersprache und
Open-Source-Ökosystem zum Quasi-Standard neben R etabliert.
Wie Python basiert R auf einer Interpreter-Laufzeitumgebung, wurde aber
von Anfang an als domänenspezifische Arbeitsumgebung für statistische
Berechnungen und Datenvisualisierung konzipiert und Wert auf die
einfache und robuste Erweiterbarkeit durch C++-Module gelegt.
Um nativ compilierte, performance-optimierte Libraries wie LAPACK in
Python einzubinden gab es bis vor wenigen Jahren nur die Möglichkeit,
diese mit C-Bindings zu kapseln und für die Python Runtime-API als Modul
bereitzustellen. Die starre und restriktive C-API machte es schwer,
den vollen Funktionsumfang einer vorhandenen Library abzubilden, und im
Fall von C++-Implementierungen in der Regel unmöglich.

Aus der Python-Entwicklergemeinschaft sind verschiedene Lösungsansätze
und Hilfsmittel entstanden, um die Entwicklung von nativen Libraries als
Python-Extensions zu erleichtern.
2016 wurde schließlich pybind11 veröffentlicht, eine robuste und
umfassende Lösung zur Integration von C++-Libraries mit expliziter
Unterstützung des C++11-Standards, dessen Neuerungen Schwerpunkt dieses
Praktikums sind.

Neben den beschriebenen programmatischen Problemen sind vor allem
konzeptionelle Unterschiede eine Herausforderung für die Abbildung von
C++-Semantiken auf die schwach getypte, interpretierte Python-Umgebung.

In Rahmen dieser Projektarbeit wurde die Verwendung benutzerdefinierter
C++-Container und Algorithmen für Python-Extensions untersucht.


## Install

Under macOS, install first with terminal command `pip install cppimport`


## Run

Open a python interpreter and run those lines:

```python
>>> import cppimport
>>> fancy = cppimport.imp("fancy")
>>> fancy.test()
```
