MAINFILE = Masterarbeit.tex
OPTIONS = --jobname=Masterarbeit

default: pdf

pdf:
	pdflatex $(OPTIONS) $(MAINFILE)

clean:
	find . \
	-path './.*' -prune -o \
	-type f \( \
	-name "*.aux" \
	-o -name "*.aux" \
	-o -name "*.backup" \
	-o -name "*.glo" \
	-o -name "*.ilg" \
	-o -name "*.ind" \
	-o -name "*.ist" \
	-o -name "*.lof" \
	-o -name "*.log" \
	-o -name "*.lol" \
	-o -name "*.lot" \
	-o -name "*.nlo" \
	-o -name "*.nls" \
	-o -name "*.out" \
	-o -name "*.toc" \
	-o -name "*.snm" \
	-o -name "*.nav" \
	-o -name "*.idx" \
	-o -name "*.*~" \
	-o -name "*~" \) \
	-print0 | xargs -0 rm
