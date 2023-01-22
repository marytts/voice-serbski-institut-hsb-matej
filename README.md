voice-serbski-institut-hsb-matej
================================

A male Upper Sorbian unit selection voice for [MaryTTS](http://mary.dfki.de/), using [data](https://github.com/marytts/serbski-institut-hsb-data) recorded at the [Sorbian Institute](https://www.serbski-institut.de/).

Building
--------

### Prerequisites

[Java](https://openjdk.org/) must be installed, as well as [SoX](https://sox.sourceforge.net/) and the [Edinburgh Speech Tools](https://www.cstr.ed.ac.uk/projects/speech_tools/).

Java installations can be easily managed via [SDKMAN!](https://sdkman.io/).

On macOS with [Homebrew](https://brew.sh/), run

    brew install sox speech-tools

On Debian/Ubuntu-based Linux, run

    sudo apt install sox speech-tools

### Git submodules

This project currently uses [Git submodules](https://git-scm.com/book/en/v2/Git-Tools-Submodules).
To ensure that they are initialized and up-to-date, run

    git submodule update --init

### Building the voice

Run

    ./gradlew build

Running
-------

To run the voice in an ad-hoc MaryTTS server, run

    ./gradlew run

Then, go to <http://localhost:59125/>.

Copyright and license
---------------------

Copyright 2022 [Sorbian Institute](https://www.serbski-institut.de/).

![CC-BY-NC-SA-4.0](https://mirrors.creativecommons.org/presskit/buttons/88x31/svg/by-nc-sa.svg)

This work is licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-nc-sa/4.0/).
