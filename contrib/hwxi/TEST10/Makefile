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
test10
test10: \
test10.dats; $(PATSCC) -o $@ $<
regress:: test10; ./test10
cleanall:: ; $(RMF) test10

## ###### ###### ##

all:: \
test11
test11: \
test11.dats; $(PATSCC) -o $@ $<
regress:: test11; ./test11
cleanall:: ; $(RMF) test11

## ###### ###### ##

all:: \
test12
test12: \
test12.dats; $(PATSCC) -o $@ $<
regress:: test12; ./test12
cleanall:: ; $(RMF) test12

## ###### ###### ##

all:: \
test13
test13: \
test13.dats; $(PATSCC) -o $@ $<
regress:: test13; ./test13
cleanall:: ; $(RMF) test13

## ###### ###### ##

all:: \
test14
test14: \
test14.dats; $(PATSCC) -o $@ $<
regress:: test14; ./test14
cleanall:: ; $(RMF) test14

## ###### ###### ##
#
all:: \
test15
test15: \
test15.dats; $(PATSCC) -tcats $<
#
## ###### ###### ##
#
all:: \
test16
test16: \
test16.dats; $(PATSCC) -tcats $<
#
## ###### ###### ##
#
all:: \
test17
test17: \
test17.dats; \
$(PATSCC) -D_GNU_SOURCE -o $@ $<
regress:: test17; ./test17
cleanall:: ; $(RMF) test17
#
## ###### ###### ##
#
all:: \
test18
test18: \
test18.dats; \
$(PATSCC) -D_GNU_SOURCE -o $@ $<
regress:: test18; ./test18
cleanall:: ; $(RMF) test18
#
## ###### ###### ##
#
all:: \
test19
test19: \
test19.dats; $(PATSCC) -tcats $<
#
## ###### ###### ##

all:: \
bternary
bternary: \
bternary.dats; \
$(PATSCC) -DATS_MEMALLOC_LIBC -o $@ $<
regress:: bternary; ./$<
cleanall:: ; $(RMF) bternary

## ###### ###### ##

all:: \
queens
queens: \
queens.dats; \
$(PATSCC) -DATS_MEMALLOC_LIBC -o $@ $<
regress:: queens; ./queens > /dev/null
cleanall:: ; $(RMF) queens

## ###### ###### ##

all:: \
palindrome
palindrome: ; $(PATSCC) -tcats palindrome.dats
all:: \
palindrome2
palindrome2: ; $(PATSCC) -tcats palindrome2.dats
all:: \
palindrome3
palindrome3: ; $(PATSCC) -tcats palindrome3.dats
all:: \
palindrome4
palindrome4: ; $(PATSCC) -tcats palindrome4.dats

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
