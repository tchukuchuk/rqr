
SHELL = /bin/sh

#### Start of system configuration section. ####

srcdir = .
topdir = /Users/jbiard/.rbenv/versions/ree-1.8.7-2011.03/lib/ruby/1.8/i686-darwin11.3.0
hdrdir = $(topdir)
VPATH = $(srcdir):$(topdir):$(hdrdir)
exec_prefix = $(prefix)
prefix = $(DESTDIR)/Users/jbiard/.rbenv/versions/ree-1.8.7-2011.03
sharedstatedir = $(prefix)/com
mandir = $(datarootdir)/man
psdir = $(docdir)
oldincludedir = $(DESTDIR)/usr/include
localedir = $(datarootdir)/locale
bindir = $(exec_prefix)/bin
libexecdir = $(exec_prefix)/libexec
sitedir = $(libdir)/ruby/site_ruby
htmldir = $(docdir)
vendorarchdir = $(vendorlibdir)/$(sitearch)
includedir = $(prefix)/include
infodir = $(datarootdir)/info
vendorlibdir = $(vendordir)/$(ruby_version)
sysconfdir = $(prefix)/etc
libdir = $(exec_prefix)/lib
sbindir = $(exec_prefix)/sbin
rubylibdir = $(libdir)/ruby/$(ruby_version)
docdir = $(datarootdir)/doc/$(PACKAGE)
dvidir = $(docdir)
vendordir = $(libdir)/ruby/vendor_ruby
datarootdir = $(prefix)/share
pdfdir = $(docdir)
archdir = $(rubylibdir)/$(arch)
sitearchdir = $(sitelibdir)/$(sitearch)
datadir = $(datarootdir)
localstatedir = $(prefix)/var
sitelibdir = $(sitedir)/$(ruby_version)

CC = /usr/bin/gcc-4.2
LIBRUBY = $(LIBRUBY_A)
LIBRUBY_A = lib$(RUBY_SO_NAME)-static.a
LIBRUBYARG_SHARED = 
LIBRUBYARG_STATIC = -l$(RUBY_SO_NAME)-static

RUBY_EXTCONF_H = 
CFLAGS   =  -fno-common -g -O2  -pipe -fno-common $(cflags) 
INCFLAGS = $(PREINCFLAGS) -I. -I/opt/local/include -I. -I/Users/jbiard/.rbenv/versions/ree-1.8.7-2011.03/lib/ruby/1.8/i686-darwin11.3.0 -I.
DEFS     = 
CPPFLAGS = -DHAVE_JPEGLIB_H -DHAVE_TIFF_H -I/opt/local/include -I'/Users/jbiard/.rbenv/versions/ree-1.8.7-2011.03/include'  -D_XOPEN_SOURCE -D_DARWIN_C_SOURCE  -I'/Users/jbiard/.rbenv/versions/ree-1.8.7-2011.03/include' 
CXXFLAGS = $(CFLAGS) 
ldflags  = -L. -L'/Users/jbiard/.rbenv/versions/ree-1.8.7-2011.03/lib' 
dldflags = 
archflag = 
DLDFLAGS = $(ldflags) $(dldflags) $(archflag)
LDSHARED = cc -dynamic -bundle -undefined suppress -flat_namespace
AR = ar
EXEEXT = 

RUBY_INSTALL_NAME = ruby
RUBY_SO_NAME = ruby
arch = i686-darwin11.3.0
sitearch = i686-darwin11.3.0
ruby_version = 1.8
ruby = /Users/jbiard/.rbenv/versions/ree-1.8.7-2011.03/bin/ruby
RUBY = $(ruby)
RM = rm -f
MAKEDIRS = mkdir -p
INSTALL = /usr/bin/install -c
INSTALL_PROG = $(INSTALL) -m 0755
INSTALL_DATA = $(INSTALL) -m 644
COPY = cp

#### End of system configuration section. ####

preload = 

libpath = . $(libdir) /opt/local/lib
LIBPATH =  -L. -L$(libdir) -L/opt/local/lib
DEFFILE = 

CLEANFILES = mkmf.log
DISTCLEANFILES = 

extout = 
extout_prefix = 
target_prefix = /rqr
LOCAL_LIBS = 
LIBS =  -lsupc++  -L/opt/local/lib -ldl -lobjc  
SRCS = qr_wrap.cxx qr_draw_jpeg.cpp qr_draw_png.cpp qr_draw_ps.cpp qr_draw_tiff.cpp QR_Encode.cpp
OBJS = qr_wrap.o qr_draw_jpeg.o qr_draw_png.o qr_draw_ps.o qr_draw_tiff.o QR_Encode.o
TARGET = QR
DLLIB = $(TARGET).bundle
EXTSTATIC = 
STATIC_LIB = 

BINDIR        = $(bindir)
RUBYCOMMONDIR = $(sitedir)$(target_prefix)
RUBYLIBDIR = /Users/jbiard/.rbenv/versions/ree-1.8.7-2011.03/gemsets/moxity-test/gems/rqr-0.2.2/lib$(target_prefix)
RUBYARCHDIR = /Users/jbiard/.rbenv/versions/ree-1.8.7-2011.03/gemsets/moxity-test/gems/rqr-0.2.2/lib$(target_prefix)

TARGET_SO     = $(DLLIB)
CLEANLIBS     = $(TARGET).bundle $(TARGET).il? $(TARGET).tds $(TARGET).map
CLEANOBJS     = *.o *.a *.s[ol] *.pdb *.exp *.bak

all:		$(DLLIB)
static:		$(STATIC_LIB)

clean:
		@-$(RM) $(CLEANLIBS) $(CLEANOBJS) $(CLEANFILES)

distclean:	clean
		@-$(RM) Makefile $(RUBY_EXTCONF_H) conftest.* mkmf.log
		@-$(RM) core ruby$(EXEEXT) *~ $(DISTCLEANFILES)

realclean:	distclean
install: install-so install-rb

install-so: $(RUBYARCHDIR)
install-so: $(RUBYARCHDIR)/$(DLLIB)
$(RUBYARCHDIR)/$(DLLIB): $(DLLIB)
	$(INSTALL_PROG) $(DLLIB) $(RUBYARCHDIR)
install-rb: pre-install-rb install-rb-default
install-rb-default: pre-install-rb-default
pre-install-rb: Makefile
pre-install-rb-default: Makefile
$(RUBYARCHDIR):
	$(MAKEDIRS) $@

site-install: site-install-so site-install-rb
site-install-so: install-so
site-install-rb: install-rb

.SUFFIXES: .c .m .cc .cxx .cpp .C .o

.cc.o:
	$(CXX) $(INCFLAGS) $(CPPFLAGS) $(CXXFLAGS) -c $<

.cxx.o:
	$(CXX) $(INCFLAGS) $(CPPFLAGS) $(CXXFLAGS) -c $<

.cpp.o:
	$(CXX) $(INCFLAGS) $(CPPFLAGS) $(CXXFLAGS) -c $<

.C.o:
	$(CXX) $(INCFLAGS) $(CPPFLAGS) $(CXXFLAGS) -c $<

.c.o:
	$(CC) $(INCFLAGS) $(CPPFLAGS) $(CFLAGS) -c $<

$(DLLIB): $(OBJS) Makefile
	@-$(RM) $@
	$(LDSHARED) -o $@ $(OBJS) $(LIBPATH) $(DLDFLAGS) $(LOCAL_LIBS) $(LIBS)



$(OBJS): ruby.h defines.h
