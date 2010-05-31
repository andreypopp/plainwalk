SRC := $(wildcard ./*.rst)
HTML := $(SRC:%.rst=%.html)

all: $(HTML)

%.html: %.rst
	rst2html.py --template=template.tpl $< > $@
