##
## A Makefile for simple testing
##

## ###### ###### ##

PATSCC=$(PATSHOME)/bin/patscc
PATSOPT=$(PATSHOME)/bin/patsopt

## ###### ###### ##

RMF=rm -f

## ###### ###### ##

all::
regress::
cleanall::

## ###### ###### ##

all:: \
test30
test30: \
test30.dats; $(PATSCC) -o $@ $<
regress:: test30; ./test30
cleanall:: ; $(RMF) test30

## ###### ###### ##

all:: \
test31
test31: \
test31.dats; $(PATSCC) -o $@ $<
regress:: test31; ./test31
cleanall:: ; $(RMF) test31

## ###### ###### ##

all:: \
test32
test32: \
test32.dats; \
$(PATSCC) -DATS_MEMALLOC_LIBC -o $@ $<
regress:: test32; ./test32
cleanall:: ; $(RMF) test32

## ###### ###### ##

all:: \
test33
test33: \
test33.dats; \
$(PATSCC) -DATS_MEMALLOC_LIBC -o $@ $<
regress:: test33; ./test33
cleanall:: ; $(RMF) test33

## ###### ###### ##

all:: \
test34
test34: \
test34.dats; \
$(PATSCC) -DATS_MEMALLOC_LIBC -o $@ $<
regress:: test34; ./test34
cleanall:: ; $(RMF) test34

## ###### ###### ##

all:: \
test35
test35: \
test35.dats; \
$(PATSCC) -DATS_MEMALLOC_LIBC -o $@ $<
regress:: test35; ./test35
cleanall:: ; $(RMF) test35

## ###### ###### ##

all:: \
test36
test36: \
test36.dats; $(PATSCC) -o $@ $<
regress:: test36; ./test36
cleanall:: ; $(RMF) test36

## ###### ###### ##
#
all:: \
test37
test37: \
test37.dats; $(PATSCC) -tcats $<
#
## ###### ###### ##

all:: \
test38
test38: \
test38.dats; \
$(PATSCC) -DATS_MEMALLOC_LIBC -o $@ $<
regress:: test38; ./test38
cleanall:: ; $(RMF) test38

## ###### ###### ##

all:: \
test39
test39: \
test39.dats; $(PATSCC) -o $@ $<
regress:: test39; ./test39
cleanall:: ; $(RMF) test39

## ###### ###### ##

all:: \
struct0
struct0: \
struct0.dats; $(PATSCC) -o $@ $<
regress:: struct0; ./struct0
cleanall:: ; $(RMF) struct0

all:: \
struct1
struct1: \
struct1.dats; $(PATSCC) -o $@ $<
regress:: struct1; ./struct1
cleanall:: ; $(RMF) struct1

## ###### ###### ##

testall:: all
testall:: regress
testall:: cleanall

## ###### ###### ##

clean:: ; $(RMF) *~
clean:: ; $(RMF) *_?ats.c

## ###### ###### ##

cleanall:: clean

## ###### ###### ##

## ###### end of [Makefile] ###### ##
