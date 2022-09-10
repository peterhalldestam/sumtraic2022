TEX=latexmk
TEXF=-pdf -pdflatex="pdflatex" -outdir="pdf"

all: auto_regression causality non_causality first_difference

auto_regression: auto_regression.pdf

causality: causality.pdf

non_causality: non_causality.pdf

first_difference: first_difference.pdf

%.pdf: %.tex
	$(TEX) $(TEXF) -use-make $<

clean:
	rm -f *.fdb_latexmk *.fls
	rm -rf pdf/*
	rmdir pdf
