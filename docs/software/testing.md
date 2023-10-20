# Sofware Testing

## Why?

* You analyzed some data and started putting the results in your paper. While writing you notice some inconsistencies in the results, you dig into your script and find out it is not doing what you expected.
* You know the output of your software is not correct. But it is difficult to figure out where in your code you made a mistake.
* You have received some code from a colleague. You have been assured it works. You start running the code, for your input you are suddenly getting errors or wildly inaccurate results.

Software testing has the following advantages:

* It improves the maintainability of your code. By automatically being able to test your software you can be more certain that you did not break anything in your code.
* It makes it easier to spot mistakes. Having automated tests can help you pinpoint where in your software you have made a mistake.
* It gives you, and others, more confidence in the correctness of the results.
* Since you define the expected inputs and outputs tests can also serve as a form of documentation. It makes clear what the expectations are for a certain piece of your software and therefore also gives some information on how it can be used.

## How?

When we talk about (automated) software testing then we define a few types of tests the main categories are:

* End-to-end tests: These test the full working of your software. In the case of a simple script this could be a test which provides an input file and checks if the expected output file is created.
* Unit tests: Unit tests test a smaller piece (unit) of your software. This can be for example a test of a single function which is used to process your results.
* Integration tests:   Integration tests test tests your integrations with 3rd party services. E.g. if your application makes use of some third party software you test if the system works as expected when you combine your code with this third party software.
* Performance tests:  As the name suggests these test the performance of the system (e.g. how fast is a certain analysis?).

When dealing with more simple research projects you are most likely interested in the first two: end-to-end tests and unit tests. When you are just starting out with automated testing we suggest focusing on end-to-end tests first as these will give you the best idea about whether your full software works as expected. Unit tests can then be used to more specifically test complex edge cases of a certain function or to pinpoint where the mistakes are in your code.

## What?
<!---TODO: add relevant links-->

### Tools

If you are working in Python, then Python has a pretty good built in testing framework for unit tests, called unittest. If you are working with jupyter notebooks then Python’s builtin framework called doctest might also be useful. The doctest framework allows you to define some simple tests in comments in your code. If you add these comments to your jupyter notebook then jupyter notebook will also complain when it detects an error in these test cases. Additionally within the Python community pytest is also commonly used, it is often seen as being more readable than the built-in unittest framework.
Usage of the tools

To start with software testing you need to consider two important questions:

* What is the expected behaviour of the software on certain inputs?
* What are the edge cases of this behaviour?
  * With this we mean: for which cases should the software do something differently than the “normal” flow. A simple example is a division function. If the divider is 0 then a division is not possible so instead an error should be thrown. In our tests we would therefore check:
    * That the correct result is produced when the divider is something different than 0.
    * That an error is thrown when the divider is 0.

If you have answered these two questions you can start creating test cases which check this behaviour and their edge cases.
Courses

Want to learn more about software testing?

* If you want to increase your software skills in general then the library offers a course which you can get graduate school credits for. This course is meant for people who already are able to program but would like to improve their skills. It also includes a part about software testing.
* If you want to learn more about advanced software testing topics then the TU Delft also offers some MOOCs on software testing. These are mostly here for people with a deep interest in software testing. We do not expect that you need the skills from these courses in your normal research.
