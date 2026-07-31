# CEFET-MG Template

![Cover](./Imagens/Capa.png)

This repository contains the LaTeX template that follows the official standards of the [University Library](https://www.bu.cefetmg.br/wp-content-uploads-sites-181-2023-04-manual-de-normalizacao-do-cefet-mg-pdf/) of CEFET.

## Execution

### Overleaf
Simply duplicate the project using this [link](https://www.overleaf.com/read/dtjckhkgjtqk) or download the repository ZIP and upload it to Overleaf.

### Local
To use it locally, make sure you have the `texlive-full` package installed on your Debian-based system or the equivalent for other operating systems.

#### Visual Studio Code
It is recommended to install the [LaTeX Workshop](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop) extension together with [Code Spell Checker](https://marketplace.visualstudio.com/items?itemName=streetsidesoftware.code-spell-checker-portuguese-brazilian) for [Visual Studio Code](https://code.visualstudio.com/) with the following configuration.

```
"latex-workshop.latex.outDir": "./.out/",
```
This keeps the project root directory clean.

#### Manually
Since this project was configured with [latexmk](https://ctan.org/pkg/latexmk?lang%253En) to maintain full compatibility with Overleaf, simply run the following command in the terminal:

```
latexmk -pdf -output-directory=out main.tex
```

## Customization
This package can be customized by passing arguments as follows:
```latex
\usepackage[acronym, glossaries, index, labelref, debug]{CEFET}
```

- **acronym:** adds support for the list of abbreviations and acronyms;
- **glossaries:** adds support for the glossary;
- **index:** adds support for the subject index;
- **labelref:** `\ref{fig:1}` returns `Figure 1` instead of `1` for all references;
- **debug:** enables rulers and frames to improve measurement visualization.
