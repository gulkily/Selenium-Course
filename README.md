Selenium-Course
===============
This is an outline of my Selenium workshop.

Prerequisites
=============
In order to save time and standardize the working environment, a virtual machine image will be provided for everyone's use that includes all of the software already preinstalled.

What is required from you is a computer with the following:

* Mac OS X, Windows, or Linux
* 4GB of RAM
* 16GB of storage
* VirtualBox already installed
* USB port

You also need to create a free account on each of the following services:

* [GitHub](http://www.github.com/)
* [SauceLabs](http://www.saucelabs.com/)
* [StackOverflow](http://www.stackoverflow.com/)
* [Reddit](http://www.reddit.com/)

In the latter stages of the course, you will also need to install the following software on your host machine. Instructions will be provided as needed:

* Java JDK 7 or later
* RemoteWebDriver server standalone executable (just download the .jar file)

Software Used
=============
* Debian GNU/Linux
* IntelliJ IDEA
* Git
* Maven
* Java
* Firefox
* Firebug
* FirePath
* Chrome or Chromium

Getting Started
===============
1. Opening the Maven project with IntelliJ
2. Running the sample test
3. Changing the browser used to run the test
4. Running an individual test
5. Was the test successful?
6. What caused the test to fail?

Running Tests and Analyzing the Results
=======================================
1. Manually run the entire test suite
2. Viewing screenshots

Planning a New Test
===================
1. What's the point of automation?
    1. Sanity checks
    2. Regression testing of previously fixed issues
    3. Detecting problems without exact specifications
2. Breaking down the test into steps
    1. Follow the manual test plan
    2. Break it down into actions

Writing a New Test
==================
1. Creating a new test class
2. Finding an element
    1. By element tag
    2. By id
    3. By class
    4. By xpath
    5. By nested structure
3. Interacting with an element
    1. Clicking
    2. Hovering
    3. Entering text
    4. Scrolling
4. Detecting changing page state
    1. Element appearance
    2. Element disappearance
    3. Page URL
    4. Element text
5. Testing for common problems
    1. Are there any broken images or links?
    2. Are there any JavaScript errors?
    3. Are any elements off-screen?
    4. Does the page include common problem words like "error"?
    5. Does the page have all of the expected content?

Using RemoteWebDriver
=====================
1. What is RemoteWebDriver?
2. Connecting to the host computer
3. Creating a SauceLabs account
4. Using RemoteWebDriver and Capabilities to specify a platform
5. Running a test
6. Practice running tests on each others' machines

Page State Fingerprinting
=========================
1. How does it work?
    1. Each element on a page, including the page itself, has properties
    2. Each property can be thought of as a data point
    3. If the data points are the same, that means the page looks the same
    4. If the data points are different, that means the page looks different
    5. Data points can be recorded in a database and compared later
2. What datapoints can be used?
    1. Dimensions and position: width, height, x and y
    2. Text and content
    3. Font color, background color, border color, etc.
    4. Border, margin, padding values
    5. Number and content of child elements
3. What is it useful for?
    1. Detecting cross-browser issues
    2. Detecting unexpected page changes
    3. Detecting layout problems

(c) 2014 Ilya Gulko