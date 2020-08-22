TEX = pandoc details.yml \
							../_includes/cv/bio.md \
							../_includes/cv/software.md \
							../_includes/cv/service.md \
							../_includes/cv/funded.md \
							../_includes/cv/awards.md \
							../_includes/cv/research.md \
							../_includes/cv/courses.md \
							../_includes/cv/mentoring.md \
							../_includes/cv/talks.md \
							../_includes/cv/tutorials.md \
							../_includes/cv/teaching-statement.md
src = template.tex
FLAGS = --pdf-engine=xelatex

resume.pdf : $(src)
	$(TEX) $(filter-out $<,$^ ) -o $@ --template=$< $(FLAGS)

.PHONY: clean
clean :
	rm resume.pdf
