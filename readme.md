BW-TEST
=======

Introduction
------------
BW-TEST is an open source library prepared to make your BusinessWorks project ready for continuous integration processes by providing an intuitive way of developing tests within TIBCO Designer. It gives you the possibility to practice TDD in TIBCO BusinessWorks and makes it possible to run your unit tests on a CI server like Jenkins.

How to use:
---------------------------------------
* Compile the library from the sources or directly pick it from the bin folder.
* Add the file alias to TIBCO Designer.
* Add a reference to the projlib in your project.
* Make your tests using the provided interface (TestProcessInput and TestProcessOutput from TESTTypes.xsd).
* Customize the Global Variables if needed.
* Run and test it from a browser or with your CI server
	by default the address is localhost:5554 for the XUnit report
	or localhost:5554/?html for HTML report
* Deploy your archive.
* Configure a job on your continuous integration server to retrieve the test results, with for example wget.
* Do something else until your CI server wakes you up!

Requirements
------------
* BusinessWorks 5.10
* Designer 5.7.4.4

Version history
---------------
v0.3
* tests and testsuites are automatically retrieved from your project. Organise your tests by putting them in folders with suffix Testsuite (e.g. MyFirstTestsuite) in your unit test location.

v0.2
* unit tests run in isolation
* specify timeout value for your tests by GV
* fixed XUnit report
* added an example test to the dtl to get started quickly

v0.1
* failure support
* error support
* multiple assertion support by using Assertions.process in your test
* test suites support
* xunit format (relaxed)
* tested on Jenkins with XUnit plugin
* XML and HTML reports
* support running on startup for doing it just once on every deploy (default)
* support running on every request

