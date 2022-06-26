FILENAME=Tarea1

# pdf: postprocess
# 	latexmk -pdflatex $(FILENAME).tex

# postprocess: convert preamble.tex
# 	sed -E -i -e '/\\fi$$/s/\\fi/\\fi\n\\usepackage{mlmodern}/' $(FILENAME).tex
# 	sed -E -i -e '/11pt/s/11pt/12pt/' $(FILENAME).tex
# 	sed -E -i -e '/article/s/article/scrartcl/' $(FILENAME).tex
# 	sed -E -i -e '/\\title/s/\\title.*/\\input{preamble.tex}/' $(FILENAME).tex
# 	sed -E -i -e '/titling/d' $(FILENAME).tex
# 	sed -E -i -e '/\\usepackage\{parskip\}/d' $(FILENAME).tex
# 	sed -E -i -e '/\\newcommand\{\\iprod\}/d' $(FILENAME).tex
# 	sed -E -i -e 's/(.*)\.png/\1\.pdf/g' $(FILENAME).tex
# 	sed -E -i -e 's/(\\maketitle)/\1\\tableofcontents/' $(FILENAME).tex
    

convert: $(FILENAME).ipynb
	jupyter nbconvert --to html $(FILENAME).ipynb

