IMAGENS=bst balanced_bst degenerated_bst kdtree

%.pdf: %.tex
	pdflatex $<

%.svg: %.pdf
	pdftocairo -svg $< $@
	$(RM) *.aux *.dvi *.pdf *.out *.log *.nav *.snm *.toc

all: $(patsubst %,%.svg,$(IMAGENS))

.PHONY: all clean

clean:
	$(RM) *.aux *.dvi *.pdf *.out *.log *.nav *.snm *.toc *.svg

