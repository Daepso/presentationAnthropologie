TEX=pdflatex
PDF=slides.pdf

all: $(PDF)

SRC=$(wildcard *.tex)
IMG=$(wildcard ./image/*.png) 

slides.pdf: slides.tex $(IMG) $(SRC)
	$(TEX) $<
	$(TEX) $<
	rm *.aux *.log *.toc *.out *.nav *.snm

.PHONY: clean display

display:
	evince $(PDF) &

clean:
	rm *.aux *.log *.toc *.out *.nav *.snm *.pdf
