ntop: netflow2ng ndpi
	cd ntopng && ./autogen.sh && ./configure && $(MAKE) && $(MAKE) install #-j4

ndpi:
	cd nDPI && ./autogen.sh --with-only-libndpi && ./configure && $(MAKE) #-j4

netflow2ng:
	cd netflow2ng && $(MAKE) -B #netflow

all: ntop
	echo "Done"
