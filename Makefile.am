bin_PROGRAMS=psplash psplash-write

AM_CFLAGS = $(GCC_FLAGS) -D_GNU_SOURCE

psplash_SOURCES = psplash.c psplash.h psplash-fb.c psplash-fb.h \
                  psplash-console.c psplash-console.h           \
		  psplash-colors.h psplash-config.h		\
		  psplash-poky-img.h psplash-bar-img.h radeon-font.h \
		  psplash-scanout.c psplash-scanout.h \
		  psplash-draw.c psplash-draw.h psplash-font.h \
		  psplash-main.c psplash-main.h \
		  psplash-fbdev.c psplash-fbdev.h \
		  psplash-kms.c psplash-kms.h \
		  psplash-drm.c psplash-drm.h

psplash_write_SOURCES = psplash-write.c psplash.h

EXTRA_DIST = make-image-header.sh
 
MAINTAINERCLEANFILES = aclocal.m4 compile config.guess config.sub configure depcomp install-sh ltmain.sh Makefile.in missing

snapshot:
	$(MAKE) dist distdir=$(PACKAGE)-snap`date +"%Y%m%d"`

