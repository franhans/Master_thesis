DATESTAMP = `/bin/date +%Y-%m-%d`

all: pdf help

pdf:
	pdflatex main
	bibtex main
	pdflatex main
	pdflatex main
	mv main.pdf ${DATESTAMP}.pdf

clean:
	rm -f  *.log *.aux *.out *.vtc *.bbl *.blg

cleanall:
	rm -f  *.log *.aux *.out *.vtc *.bbl *.blg *.pdf

help:
	@echo "Help: Other Commands"
	@echo "\tmake pdf"
	@echo "\tmake clean"


