all: clean main

view:
	evince main.pdf &

main: main.tex *.tex
	pdflatex main.tex
#	makeglossaries main.glo
	bibtex main.aux
	bibtex main.aux
	pdflatex main.tex
	pdflatex main.tex

clean:
	rm -f main.aux main.glg main.glo main.gls main.ist main.lof main.log main.lot main.out main.toc main.bbl main.blg main.equ main.pdf main.vtc
	rm -f doc/*.aux other/*.aux
