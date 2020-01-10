TEX = pandoc details.yml 
src = template.tex
FLAGS = 

resume.tex: $(src)
	$(TEX) $(filter-out $<,$^ ) -o $@ --template=$< $(FLAGS)

.PHONY: clean
clean :
	rm resume.tex
