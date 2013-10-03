doc=general-exam

%.pdf : %.tex
	pdflatex $<

default: $(doc).pdf
	open $(doc).pdf

clean:
	-rm -f $(talk).{aux,log,nav,out,snm,toc,vrb}
	-rm -f ./*~

clobber: clean
	-rm -f ./*.pdf