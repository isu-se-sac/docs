TEX=$(wildcard *.tex)
PDF=$(TEX:.tex=.pdf)
AUX=$(TEX:.tex=.aux)
LOG=$(TEX:.tex=.log)
OUT=$(TEX:.tex=.out)

all:${PDF}

${PDF}:%.pdf:%.tex
	pdflatex $<
	pdflatex $<
	rm -f ${AUX} ${LOG} ${OUT}

clean:
	rm -rf ${PDF}

.PHONY: clean
