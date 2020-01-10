DESTDIR =
DICTDIR = /usr/share/myspell/dicts
DICTIONARYLIST = $(DICTDIR)/dictionary.lst

INSTALL      = install -m755
INSTALL_DATA = install -m644

all:

install:
	$(INSTALL) -d $(DESTDIR)$(DICTDIR)
	$(INSTALL_DATA) se.aff se.dic $(DESTDIR)$(DICTDIR)/.
	cat hunspell-se >> $(DESTDIR)$(DICTIONARYLIST)
	cd $(DESTDIR)$(DICTDIR) && \
	ln -s se.dic se_FI.dic && \
	ln -s se.aff se_FI.aff && \
	ln -s se.dic se_NO.dic && \
	ln -s se.aff se_NO.aff && \
	ln -s se.dic se_SE.dic && \
	ln -s se.aff se_SE.aff

clean:
