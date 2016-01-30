SRC=resume
REPO=itmeson@buphy.bu.edu:public_html/REPOS/Jobs/RESUME/
DATE=$(shell date +%Y-%m-%d)

build: lat lat pdf
	cp resume.pdf betnel_resume.pdf

lat:
	latex $(SRC).tex 


pdf:
	dvipdf $(SRC).dvi $(SRC).pdf


