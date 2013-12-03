BW-TEST
=======

Introduction
------------
BW-TEST is an open source library prepared to make your businesswork project ready to continuous integration processes by providing an intuitive way of developing tests within TIBCO Designer, allowing the use of jenkins for example, and giving you the possibility to practice TDD in TIBCO BusinessWorks. Remember: write the test, add some code, refactor!
Now you and your customers can enjoy a better quality ESB in their organizations and they can also save time and money.

Getting started
---------------
* Read the Big picture how to
* See the video
* Constantly view the example code

Big picture how to: use
---------------------------------------
* compile the library from the sources or directly pick it from the bin folder here
* add the file alias
* add a reference to the projlib from your project
* dev your tests using the provided interface (TestProcessInput and TestProcessOutput from TESTTypes.xsd)
* build your test.xml
* customize the variables
* run and test it from a browser or with your ci server
	by default the address is localhost:5554 for the XUnit report
	or localhost:5554/?html for HTML report
* depoy your archive
* configure your job in your continuous integration server
	tip: if your jenkins is under ubuntu for example, you can use wget
	tip 2: on windows you can use it too by installing unix tools provided with for example git
* go to do something else until your ci server wakes you up!

Requirements
------------
* BusinessWorks 5.10
* Designer 5.7.4.4

Version history
---------------
v0.1
* failure support
* error support
* multiple assertion support by using Assertions.process once in your test
* test suites support
* xunit format (relaxed)
* tested on jenkins with xunit plugin
* xml and html reports
* support startup running for doing it just once on every deploy (default)
* support running on every request

