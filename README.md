OUTemplate
==========

Open Universiteit Latex Template

Using the template
------------------

This is the OU LaTeX template provided by Patrick Molijn.
Minor changes are provided by Ed van Doorn
It is designed to work with all versions of LaTeX, but is primarily used with pdflatex.
The document can be compiled with

  rm *.aux *.acn *.acr *alg *.bbl *.bcf *.blg *.dvi *glg *.gls *.glsdefs *.glo *.ist *.log *.lot *.lof *.out *run.xml *.toc *.synctex.gz *~ 2>/dev/null
  # Linux command to remove files.
  pdflatex report
  bibtex report
  pdflatex report
  pdflatex report
  # It is really necessary to call pdflatex twice.

A separate example document is available which generates a cover image (front,
back and spine). This document can be generated with

  pdflatex cover
  pdflatex cover

or simply with the 'pdfLaTeX' option in the TeX editing program.


Installation on Windows
-----------------------

The template has been tested to work with the most recent version
of MiKTeX at the time of this writing (2.9). The following packages are required
on top of a basic MiKTeX installation to make full use of the template:

  caption, fancyhdr, filehook, footmisc, fourier, l3kernel, l3packages,
  metalogo, mptopdf, ms, natbib, pgf, realscripts, tipa, titlesec, tocbibind,
  unicode-math, url, xcolor, xetex-def

Note that MiKTeX will generally automatically install these packages if they are
missing from your installation.



Installation on Linux (Debian/Ubuntu)
-------------------------------------

Recent versions of Debian, and derived distributions such as Ubuntu, use the TeX
Live system. Install the following packages to make full use of the this
template:

  texlive, texlive-fonts-extra, texlive-math-extra, texlive-lang-dutch
  (or texlive-lang-european), texlive-lang-english, texlive-latex-extra,
  texlive-xetex


 Recommand editor, websites
 --------------------------
 Open source editor: Texstudio (http://www.texstudio.org/)
 
 Latex home page: http://www.latex-project.org/
 Tutorials/help:  http://www.win.tue.nl/latex/documentation/manual.pdf
 	    	  http://www.latex-project.org/guides/usrguide.pdf
 	    	  https://tobi.oetiker.ch/lshort/lshort.pdf
	    	  http://www.it.uom.gr/teaching/latex/latex/index.html
		  http://www.bibtex.org/Using/
		  http://www.ntg.nl/maps/30/15.pdf
		  https://www.economics.utoronto.ca/osborne/latex/BIBTEX.HTM
		  https://en.wikibooks.org/wiki/LaTeX/Bibliography_Management
		  https://en.wikibooks.org/wiki/LaTeX/Mathematics

		  
Content report.tex
------------------
report.tex contains a number of settings, i.e. locations of summaries, chapters,
bibliography (APA, Plain, ..)
Pay attention to command \input{} i.e. \input{biblio/report.bib}
report.tex also contains your name    : \author{}
                         your  number : Student & number
			 and other data
			 

Make often backups
------------------
www.xp-dev.com offers free repositories for git and svn.
Store at least one backup outside your working area.
Better save than sorry.
