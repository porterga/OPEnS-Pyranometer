FILENAME = Tech_review_Garen-Porter

$(FILENAME).pdf: $(FILENAME).ps
	ps2pdf $(FILENAME).ps

$(FILENAME).ps: $(FILENAME).dvi
	dvips $(FILENAME).dvi

$(FILENAME).dvi: $(FILENAME).tex
	latex --verbose $(FILENAME).tex

clean:
		rm -f *.pdf *.ps *.dvi *.out *.log *.aux *.bbl *.blg *.pyg
