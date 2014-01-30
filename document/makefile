doc=general-exam

# %.pdf : %.tex
# 	pdflatex $<

default:
	pdflatex $(doc).tex
	bibtex $(doc)
	pdflatex $(doc).tex
	pdflatex $(doc).tex
	open $(doc).pdf

clean:
	-rm -f $(doc).{aux,log,nav,out,snm,toc,vrb,bbl,blg}
	-rm -f ./*~

clobber: clean
	-rm -f ./*.pdf
