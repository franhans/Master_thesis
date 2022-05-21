all: clean main

view:
	evince main.pdf &

main: main.tex *.tex
	pdflatex main.tex
	bibtex main.aux
	bibtex main.aux
	pdflatex main.tex
	pdflatex main.tex

clean:
	rm -f main.aux main.glg main.glo main.gls main.ist main.lof main.log main.lot main.out main.toc main.bbl main.blg main.equ
	rm -f doc/*.aux other/*.aux
