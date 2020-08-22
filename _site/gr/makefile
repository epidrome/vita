TEX = pandoc details.yml more-details.md annotated.md
src = template.tex
FLAGS = 

resume.tex : $(src)
	$(TEX) $(filter-out $<,$^ ) -o $@ --template=$< $(FLAGS)
 
.PHONY: clean
clean :
	rm resume.tex
