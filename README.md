# LaTeX-Vorlage zur Projektdokumentation für Fachinformatiker Anwendungsentwicklung

Die Vorlage umfasst neben dem Layout und den obligatorischen Elementen wie Deckblatt, Verzeichnissen und Literaturangaben insbesondere eine Vorstrukturierung der üblicherweise geforderten Inhalte einer Dokumentation zur betrieblichen Projektarbeit inklusive einiger Beispiele für wichtige Inhalte wie z.B. Kostenkalkulation und Amortisationsrechnung. Obwohl viele Inhalte der Vorlage speziell auf Anwendungsentwickler zugeschnitten sind, dürfte die Vorlage auch für die anderen IT-Berufe (Fachinformatiker Systemintegration, IT-Kaufleute usw.) interessant sein, da die Vorgaben hinsichtlich der Projektarbeit größtenteils übereinstimmen.

Mehr Informationen und eine Beispieldokumentation auf Basis dieser Vorlage gibt es hier: [Vorlage für die Projektdokumentation][fiaevorlage].

[fiaevorlage]: http://fiae.link/LaTeXVorlageFIAE "Vorlage für die Projektdokumentation"

## Prerequisites

- LaTeX distribution
    - e.g. [MiKTeX](https://miktex.org/howto/install-miktex)
        - requires a Perl distribution
            - e.g. [ActivePerl](https://www.activestate.com/products/perl/downloads/)
                - make sure the installer adds the folder containing the executable to the `PATH`
- Editor with support for LaTeX
    - e.g. [Visual Studio Code](https://code.visualstudio.com/) with the [LaTeX Workshop Extension](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop)

## Troubleshooting

### Build fails with `LaTeX fatal error: spawn latexmk ENOENT, . PID: undefined.`

This means LaTeX Workshop couldn't locate the LaTeX executables on the `PATH`. Close and then re-open ALL Visual Studio Code windows. If the problem still persists, make sure you have a LaTeX distribution installed and added the folder containing the executables to the `PATH`.

### Build fails with `latexmk: The script engine could not be found.`

This means `latexmk` couldn't locate `perl.exe` on the `PATH`. Close and then re-open ALL Visual Studio Code windows. If the problem still persists, make sure you have a Perl distribution installed and added the folder containing the executable to the `PATH`.

### First Build takes a really long time to complete

This is normal, if you're using MiKTeX, because it needs to download all required packages. But make sure you haven't overlooked any package install dialog from MiKTeX, which is still open. Because in that case the build waits as long as that dialog is open. And unless you've allowed MiKTeX to install packages without asking, this dialog will open back up each time a package needs to be installed.

## Lizenz

[![Creative Commons Lizenzvertrag](https://i.creativecommons.org/l/by-sa/4.0/88x31.png)](http://creativecommons.org/licenses/by-sa/4.0/)
LaTeX-Vorlage zur IHK-Projektdokumentation für Fachinformatiker Anwendungsentwicklung von [Stefan Macke](http://fiae.link/LaTeXVorlageFIAE) ist lizenziert unter einer [Creative Commons Namensnennung - Weitergabe unter gleichen Bedingungen 4.0 International Lizenz](http://creativecommons.org/licenses/by-sa/4.0/).
