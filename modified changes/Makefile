all: main.tex bibliography.bib
	pdflatex -interaction=nonstopmode main.tex || true
	bibtex main
	pdflatex -interaction=nonstopmode main.tex || true
	pdflatex -interaction=nonstopmode main.tex || true
