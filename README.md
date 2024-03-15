

# Thesis Template

## Getting started

### Windows

 - Prerequisits 
	 - `winget install miktex`
	 - `winget install python.python.3.12` (Add python to PATH)
	 - `pip install Pygments`
 - TexStudio
	 - winget install texstudio`
	 - open TexStudio
	 - options -> configure texstudio -> commands
	 - change PdfLaTex command to `pdflatex.exe -synctex=1 -shell-escape -interaction=nonstopmode %.tex`	 
 

Basic template for reports, bachelor and master theses at the [Technische Hochschule Nürnberg Georg Simon Ohm](https://www.th-nuernberg.de/).
It is set up to be printed as a book including a coverpage.

Extendet template with some quality of live commands and fancy code highlighting


## Important!

You need to download, fill and save-as-pdf the official [statement and copyright form](https://intern.ohmportal.de/fileadmin/Gelenkte_Doks/Abt/SZS/SB/SB_0050_FO_Pruefungsrechtliche_Erklaerung_und_Erklaerung_zur_Veroeffentlichung_der_Abschlussarbeit_public.pdf), in its most recent version.
It will be included in the final `thesis.pdf`.


## Requirements
- install [Pygments](https://pygments.org) and make sure the python scripts dir is in your path variable
- use shell-escape when calling pdf latex. pdflatex example: `pdflatex -synctex=1 -interaction=nonstopmode --shell-escape %.tex`

## A few tips for writing your thesis:

- Create a branch for your thesis; this allows you to easily sync with upstream (this repository).
- Disable automatic hard line wrap (with newlines); use soft wrap instead. [(What's that about?)](https://stackoverflow.com/questions/319925/difference-between-hard-wrap-and-soft-wrap)
- Write one sentence per line -- this makes for nice diffs in git.
- For capitalization of headlines etc., follow the [IEEE Style Manual](https://journals.ieeeauthorcenter.ieee.org/your-role-in-article-production/ieee-editorial-style-manual/)
- Use UTF-8 encoding on your files to make special characters wörk.
- Keep your literature up to date -- add references to your bib file as you read them.


## Other resources regarding your thesis

- [Informationen und Vorlagen](https://intern.ohmportal.de/institutionen/fakultaeten/informatik/studierende/infos-zum-studium/abschlussarbeiten/informationen-und-vorlagen/page.html) (German, Ohm intranet)
- [Wie schreibe ich eine Abschlussarbeit](https://www.in.th-nuernberg.de/Professors/Weber/Abschlussarbeit%20Methodik.pdf) by Prof. Dr. Rainer Weber (German, Ohm intranet).
