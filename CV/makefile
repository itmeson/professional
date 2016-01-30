SRC=cv
WEBREPO=~/Sites/markbetnel/files/
REPO=itmeson@buphy.bu.edu:public_html/REPOS/Jobs/CV/
REPO2=itmeson@itmeson.dyndns.org:Documents/research/ReviewCh/
REPO3=itmeson@crimson.physics.drexel.edu:/data/B/itmeson/Documents/ReviewCh/
DATE=$(shell date +%Y-%m-%d)

all: build sync text

build: lat lat pdf
	cp cv.pdf betnel_cv.pdf

text: build
	./maketext 

lat:
	latex $(SRC).tex 

sync:
	rsync -avz betnel_cv.pdf $(WEBREPO)

pdf:
	dvipdf $(SRC).dvi $(SRC).pdf


