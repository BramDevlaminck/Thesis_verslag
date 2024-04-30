all: abstract thesis

thesis:
	latexmk -pdflatex=lualatex --shell-escape -pdf -quiet -output-directory="../out" -jobname="thesis" main.tex

abstract:
	latexmk -cd ../abstract/abstract.tex -pdflatex=lualatex --shell-escape -pdf -quiet -output-directory="../out"

clean:
	latexmk -c -output-directory="../out" -jobname="thesis" main.tex
	latexmk -c -output-directory="../out" -cd ../abstract/abstract.tex