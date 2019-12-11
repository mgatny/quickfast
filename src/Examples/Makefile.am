LIBQUICKFASTDIR = $(top_builddir)/src

AM_CXXFLAGS = -I$(LIBQUICKFASTDIR)

noinst_LTLIBRARIES = libinterpret_application.la
libinterpret_application_la_SOURCES = \
  Examples/ValueToFix.h \
	Examples/ConsoleLock.h \
	Examples/StopWatch.h \
	Examples/MessageInterpreter.h \
	Examples/MessagePerformance.h \
	Examples/ExamplesPch.h \
	Examples/ConsoleLock.cpp \
  Examples/ExamplesPch.cpp \
  Examples/MessageInterpreter.cpp \
  Examples/MessagePerformance.cpp \
  Examples/ValueToFix.cpp \
	InterpretApplication/InterpretApplication.cpp

bin_PROGRAMS = interpret_application
interpret_application_LDADD = libinterpret_application.la $(LIBQUICKFASTDIR)/libQuickFAST.la -lxerces-c -l:libboost_filesystem.so.1.58.0 -lboost_system -lboost_thread -lpthread
interpret_application_SOURCES = InterpretApplication/main.cpp
