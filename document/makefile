doc=general-exam
LATEX=pdflatex
BIBTEX=bibtex
# %.pdf : %.tex
# 	pdflatex $<

default:
	$(LATEX) $(doc).tex
	$(BIBTEX) $(doc)
	$(LATEX) $(doc).tex
	$(LATEX) $(doc).tex
	open $(doc).pdf

clean:
	-rm -f $(doc).{aux,log,nav,out,snm,toc,vrb,bbl,blg}
	-rm -f ./*~

clobber: clean
	-rm -f ./*.pdf
