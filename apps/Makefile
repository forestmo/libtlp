CC = gcc
INCLUDE := -I../include 
LDFLAGS := -L../lib 
LDLIBS  := -ltlp -lpthread
CFLAGS  := -g -Wall $(INCLUDE)

PROGNAME = example dma_read dma_write psmem process-list pgd-walk codedump \
	   tlpperf pcie_cfg_read pcie_cfg_write

all: $(PROGNAME)

.c.o: util.h
	$(CC) $< -o $@

clean:
	rm -rf *.o
	rm -rf $(PROGNAME)
