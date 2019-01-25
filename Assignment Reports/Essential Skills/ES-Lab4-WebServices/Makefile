PROJECT?=main
FLAGS=-interaction=batchmode
OPT=--no-pdf

.PHONY: all
.PHONY: clean
.PHONY: clean-all

all:
	xelatex $(OPT) $(FLAGS) $(PROJECT).tex 
	bibtex  $(PROJECT).aux 
	xelatex $(OPT) $(FLAGS) $(PROJECT).tex 
	xelatex $(FLAGS) $(PROJECT).tex 

clean:
	rm -f *.log *.bak *.aux *.bbl *.blg *.idx *.toc *.out *.xdv *~ *.lof *.lot


clean-all:
	rm -f *.dvi *.log *.bak *.aux *.bbl *.blg *.idx *.ps *.eps *.pdf *.toc *.out *~ *.lof *.lot *.xdv
