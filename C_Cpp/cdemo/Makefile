DIRS = lib apue demo unpv13e stanet coap jpg
#DIRS = lib coap
OUT_DIR = out

all:
	test -d $(OUT_DIR) || mkdir -p $(OUT_DIR)
	@for i in $(DIRS); do \
		(cd $$i && echo "making $$i" && $(MAKE) ) || exit 1; \
	done
	@echo "Success"

clean:
	@for i in $(DIRS); do \
		(cd $$i && echo "cleaning $$i" && $(MAKE) clean) || exit 1; \
	done
	rm -rf ./out/*