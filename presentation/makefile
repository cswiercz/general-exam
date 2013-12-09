talk=general-exam

%.pdf : %.tex
	pdflatex $<
#	pdflatex $<

default: $(talk).pdf
	open $(talk).pdf

clean:
	-rm -f $(talk).{aux,log,nav,out,snm,toc,vrb}
	-rm -f ./*~

clobber: clean
	-rm -f ./*.pdf