include $(GNUSTEP_MAKEFILES)/common.make

ADDITIONAL_CFLAGS = -DBUILDING_SELF_BORON -Wno-elaborated-enum-base
ADDITIONAL_CXXFLAGS = -DBUILDING_SELF_BORON -Wno-elaborated-enum-base
ADDITIONAL_OBJCFLAGS = -DBUILDING_SELF_BORON

PACKAGE_NAME = gnustep-boron
SUBPROJECT_NAME = BoronTypes

$(SUBPROJECT_NAME)_C_FILES = \
  PlistParser.c \
  UTI.c \
  Cache.c \
  Base32.c
$(SUBPROJECT_NAME)_OBJC_FILES = ConstantExports.m Loader.m

$(SUBPROJECT_NAME)_HEADER_FILES = UTType.h UTCoreTypes.h LaunchServices.h

$(SUBPROJECT_NAME)_INCLUDE_DIRS = -I../../Headers
$(SUBPROJECT_NAME)_HEADER_FILES_DIR = ../../Headers/LaunchServices
$(SUBPROJECT_NAME)_HEADER_FILES_INSTALL_DIR = LaunchServices

$(SUBPROJECT_NAME)_NEEDS_GUI = NO

include $(GNUSTEP_MAKEFILES)/subproject.make
-include Makefile.postamble
