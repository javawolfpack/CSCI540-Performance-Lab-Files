YEAR=Spring2013

writeup-$(YEAR).pdf: writeup.tex
	pdflatex writeup.tex
	mv writeup.pdf writeup-$(YEAR).pdf

clean:
	- (cd perf-setup; make clean)
	- (cd perf-soln; make clean)
	-rm writeup.dvi writeup.aux writeup.log
	-rm perflab-setup.zip

zip:
	-rm perflab-setup.zip
	zip -r perflab-setup.zip perflab-setup
