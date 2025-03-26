all: ntop
	echo "Done"

ntop: netflow2ng ndpi
	cd ntopng && ./autogen.sh && ./configure && $(MAKE) && $(MAKE) install

ndpi:
	cd nDPI && ./autogen.sh --with-only-libndpi && ./configure && $(MAKE)

netflow2ng:
	cd netflow2ng && $(MAKE)
