#------------------------------------------------------------------------------
# CSparse Makefile
#------------------------------------------------------------------------------

VERSION = 3.1.3

C:
	( cd Lib ; $(MAKE) )

all: C cov

library:
	( cd Lib ; $(MAKE) )

cov:
	( cd Tcov ; $(MAKE) )

clean:
	( cd Lib ; $(MAKE) clean )
	( cd Tcov ; $(MAKE) clean )
	( cd MATLAB/CSparse ; $(RM) *.o )
	( cd MATLAB/Test    ; $(RM) *.o )

purge:
	( cd Lib ; $(MAKE) purge )
	( cd Tcov ; $(MAKE) purge )
	( cd MATLAB/CSparse ; $(RM) *.o *.mex* )
	( cd MATLAB/Test    ; $(RM) *.o *.mex* )

distclean: purge

# do not install CSparse; use CXSparse instead
install:

# uninstall CSparse: do nothing
uninstall:

