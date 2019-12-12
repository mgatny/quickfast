LIBQUICKFASTDIR = $(top_builddir)/src
LIBEXAMPLESLIBS = libexamples.la $(LIBQUICKFASTDIR)/libQuickFAST.la -lxerces-c -lboost_system -lboost_thread

AM_CXXFLAGS = -I$(LIBQUICKFASTDIR)

noinst_LTLIBRARIES = libexamples.la
libexamples_la_SOURCES = \
  Examples/ValueToFix.h           \
	Examples/ConsoleLock.h          \
	Examples/StopWatch.h            \
	Examples/MessageInterpreter.h   \
	Examples/MessagePerformance.h   \
	Examples/ExamplesPch.h          \
	Examples/ConsoleLock.cpp        \
  Examples/ExamplesPch.cpp        \
  Examples/MessageInterpreter.cpp \
  Examples/MessagePerformance.cpp \
  Examples/ValueToFix.cpp

bin_PROGRAMS = interpret_application tutorial_application file_to_multicast file_to_tcp pcap_to_multicast performance_test

interpret_application_LDADD = $(LIBEXAMPLESLIBS)
interpret_application_SOURCES = InterpretApplication/InterpretApplication.cpp InterpretApplication/main.cpp

tutorial_application_LDADD = $(LIBEXAMPLESLIBS)
tutorial_application_SOURCES = TutorialApplication/TutorialApplication.h TutorialApplication/TutorialApplication.cpp TutorialApplication/main.cpp

file_to_multicast_LDADD = $(LIBEXAMPLESLIBS)
file_to_multicast_SOURCES = FileToMulticast/FileToMulticast.h FileToMulticast/FileToMulticast.cpp FileToMulticast/main.cpp

file_to_tcp_LDADD = $(LIBEXAMPLESLIBS)
file_to_tcp_SOURCES = FileToTCP/FileToTCP.h FileToTCP/FileToTCP.cpp FileToTCP/main.cpp

pcap_to_multicast_LDADD = $(LIBEXAMPLESLIBS)
pcap_to_multicast_SOURCES = PCapToMulticast/PCapToMulticast.h PCapToMulticast/PCapToMulticast.cpp PCapToMulticast/main.cpp

performance_test_LDADD = $(LIBEXAMPLESLIBS)
performance_test_SOURCES = \
  PerformanceTest/MessageCounter.h    \
  PerformanceTest/NullMessage.h       \
  PerformanceTest/PerformanceTest.h   \
  PerformanceTest/MessageCounter.cpp  \
  PerformanceTest/NullMessage.cpp     \
  PerformanceTest/PerformanceTest.cpp \
  PerformanceTest/main.cpp
