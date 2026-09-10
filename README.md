Drehbank Einweisung
===================

Einweisung des [FAU FabLab](https://fablab.fau.de) in die [Drehbank](https://fablab.fau.de/tool/cnc-drehbank).

Die neueste Version der Einweisung aus [github](https://github.com/fau-fablab/drehbank-einweisung) ist als PDF unter
https://brain.fablab.fau.de/build/drehbank-einweisung/Einweisung_Drehbank.pdf
abrufbar und wird automatisch alle 20 Minuten aktualisiert.

auschecken
----------

```bash
git clone --recursive git@github.com:fau-fablab/drehbank-einweisung.git
```

bauen mit Docker
----------------

Statt LaTeX lokal zu installieren, kann der Build auch in einem Docker-Container
mit der offiziellen [`texlive/texlive`](https://hub.docker.com/r/texlive/texlive)
Image laufen:

```bash
docker run --rm -v "$PWD":/workdir -w /workdir texlive/texlive:latest make
```

Die fertigen PDFs landen anschließend im Ordner `output/`.

Technische Details zum Buildserver siehe auf macgyver `/home/buildserver/README`

[![Build Status](https://brain.fablab.fau.de/build/drehbank-einweisung/status.svg)](https://brain.fablab.fau.de/build/drehbank-einweisung/)
[![TODOs](https://brain.fablab.fau.de/build/drehbank-einweisung/status-todos.svg)](https://brain.fablab.fau.de/build/drehbank-einweisung/)

Lizenz
------

[![Lizenz: 3.0](https://licensebuttons.net/l/by-sa/3.0/de/88x31.png)</br>CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/)
