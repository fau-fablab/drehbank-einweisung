Drehbank Einweisung
===================

Einweisung des [FAU FabLab](https://fablab.fau.de) in die [CNC-Drehbank](https://fablab.fau.de/tool/zerspanung/cnc-drehbank/) Wabeco CC-D6000hs.

Inhalt
------

- Einweisungsstufen (Grund-Einweisung, CNC-Betrieb, Handbetrieb)
- Grundlagen der Zerspanung: Drehmeißel, Spannfutter und -backen, Kühlschmierstoff, Schnittwerte
- Sicherheit und Verhaltensregeln, Betriebsanweisung
- Handdrehen: Zentrieren, Bohren, Außen-/Innendrehen, Fasen, Plandrehen, Abstechen, Gegenspannen, Rändeln
- CNC: Datenerstellung mit Inventor HSM oder Siemens NX, Steuerung mit LinuxCNC
- Wartungspläne pro Quartal und Jahr

Download
--------

Die neueste Version aus [GitHub](https://github.com/fau-fablab/drehbank-einweisung) ist als PDF abrufbar:

- [Einweisung](https://brain.fablab.fau.de/build/drehbank-einweisung/Einweisung_Drehbank.pdf)
- [Einweisungsliste](https://brain.fablab.fau.de/build/drehbank-einweisung/Einweisungsliste_Drehbank.pdf)
- [Betriebsanweisung](https://brain.fablab.fau.de/build/drehbank-einweisung/Betriebsanweisung_Drehen.pdf) (Aushang)
- [Wartungsplan Quartal](https://brain.fablab.fau.de/build/drehbank-einweisung/Wartungsplan_Quartal.pdf)
- [Wartungsplan Jahr](https://brain.fablab.fau.de/build/drehbank-einweisung/Wartungsplan_Jahr.pdf)

Außerdem baut eine GitHub Action die PDFs bei jedem Push. Auf dem Hauptbranch entsteht dabei ein
[Release](https://github.com/fau-fablab/drehbank-einweisung/releases) mit Datums-Version (`vJJJJ.MM.TT`) und den PDFs.

Auschecken und bauen
--------------------

```bash
git clone --recursive git@github.com:fau-fablab/drehbank-einweisung.git
cd drehbank-einweisung
make
```

Die PDFs landen in `output/`. Layout, Kopf- und Fußzeile und das Logo des FAU FabLab (mit
FAU-Schriftzug) kommen aus dem Untermodul [fablab-document](https://github.com/fau-fablab/fablab-document),
das Logo wiederum aus dessen Untermodul [logo](https://github.com/fau-fablab/logo). Bei einem bestehenden
Klon die Untermodule mit `git submodule update --init --recursive` laden.

Technische Details zum Buildserver: [fau-fablab/buildserver](https://github.com/fau-fablab/buildserver)

[![Build Status](https://brain.fablab.fau.de/build/drehbank-einweisung/status.svg)](https://brain.fablab.fau.de/build/drehbank-einweisung/)
[![TODOs](https://brain.fablab.fau.de/build/drehbank-einweisung/status-todos.svg)](https://brain.fablab.fau.de/build/drehbank-einweisung/)
[![PDF bauen](https://github.com/fau-fablab/drehbank-einweisung/actions/workflows/pdf.yml/badge.svg)](https://github.com/fau-fablab/drehbank-einweisung/actions/workflows/pdf.yml)

Lizenz
------

[![Lizenz: CC BY-SA 3.0](https://licensebuttons.net/l/by-sa/3.0/de/88x31.png)</br>CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/)
