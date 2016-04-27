SRC = report

CLS = 

STY = 

all: pdf cleanup FORCE

pdf: FORCE
	pdflatex $(SRC).tex $(CLS) $(STY)
	bibtex $(SRC).aux
	pdflatex $(SRC).tex $(CLS) $(STY)
	pdflatex $(SRC).tex $(CLS) $(STY)

FORCE:

cleanup: FORCE
	$(RM) *.aux *.log  *.blg *.synctex.gz *.dvi *.bbl *.toc

clean: FORCE
	$(RM) *.aux *.log  *.blg *.synctex.gz *.dvi *.bbl sh.exe.stackdump *.pdf *.toc