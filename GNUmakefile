# --------------------------------------------------------------
# GNUmakefile for examples module.  Gabriele Cosmo, 06/04/98.
# --------------------------------------------------------------

name := NeutronSim
G4TARGET := $(name)
G4EXLIB := true

ifndef G4INSTALL
  G4INSTALL = ../../..
endif

.PHONY: all
all: lib bin

include $(G4INSTALL)/config/binmake.gmk

# ROOT support
CPPFLAGS += -I$(shell root-config --incdir)
EXTRALIBS = $(shell root-config --glibs)

visclean:
	rm -f g4*.prim g4*.eps g4*.wrl
	rm -f .DAWN_*

