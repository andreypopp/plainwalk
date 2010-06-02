SRC := $(wildcard ./*.rst)
HTML := $(SRC:%.rst=%.html)

all: $(HTML)

clean:
	rm -rf $(HTML)

%.html: %.rst
	rst2html.py --template=template.tpl --initial-header-level=2 $< > $@
