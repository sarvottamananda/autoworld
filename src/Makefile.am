LDADD = ../lib/libcommon.a  -lGL -lGLEW -lglfw  -lpng -lm
AM_CPPFLAGS = -DDEBUG -I$(srcdir)/../lib
AM_CFLAGS = 

COMMON_FILES = a-defs.h \
	../lib/debug.h \
	z-gui.h z-glfw.h z-options.h z-util.h z-list.h \
	z-gui.c z-glfw.c z-options.c z-util.c z-list.c \
	z-png.h z-opengl.h z-shader.h z-pvm.h z-maths.h \
	z-png.c z-opengl.c z-shader.c z-pvm.c z-maths.c \
	z-camera.h z-models.h z-materials.h z-world.h z-light.h \
	z-camera.c z-models.c z-materials.c z-world.c z-light.c \
	z-geom.h \
	z-geom.c \
	a-main.c \
	z-main.h 

PROGRAM_FILES = tut0.c tut1.c tut2.c tut3.c tut4.c tut5.c

indent: $(COMMON_FILES) $(PROGRAM_FILES)
	@echo "Indenting all source and header files"
	indent -linux -i4 -l80 -c40 -cd40 -cp33 $?

clean-local:
	-rm -f *~

bin_PROGRAMS = tut0 tut1 tut2 tut3 tut4 tut5

tut0_SOURCES = tut0.c

tut1_SOURCES = $(COMMON_FILES) \
	tut1.c

tut2_SOURCES = $(COMMON_FILES) \
	tut2.c

tut3_SOURCES = $(COMMON_FILES) \
	tut3.c

tut4_SOURCES = $(COMMON_FILES) \
	tut4.c

tut5_SOURCES = $(COMMON_FILES) \
	tut5.c
