export QUICKFAST_ROOT = $(top_builddir)
LIBQUICKFASTDIR = $(top_builddir)/src

check_PROGRAMS = unit_tests
unit_tests_CXXFLAGS = -I$(LIBQUICKFASTDIR) -DBOOST_TEST_DYN_LINK
unit_tests_LDADD = $(LIBQUICKFASTDIR)/libQuickFAST.la -lxerces-c -lboost_system -lboost_thread -lboost_unit_test_framework
unit_tests_SOURCES = \
  testAsynchSender.cpp      \
  testBiggestValue.cpp      \
  testCommon.cpp            \
  testErrorRecovery.cpp     \
  testFieldInstructions.cpp \
  testFieldOperations.cpp   \
  testGroupReferences1.cpp  \
  testGroupReferences.cpp   \
  testIntegerFields.cpp     \
  testNestedSequences.cpp   \
  testPresenceMap.cpp       \
  testReplaceField.cpp      \
  testRoundTrip1.cpp        \
  testRoundTrip.cpp         \
  testRoundTripFieldOps.cpp \
  testSequences.cpp         \
  testSmallestValue.cpp     \
  testStringFields.cpp      \
  testTemplateRef.cpp       \
  testXMLTemplateParser.cpp \
  FieldInstructionMock.h    \
  main.cpp

TESTS = unit_tests
