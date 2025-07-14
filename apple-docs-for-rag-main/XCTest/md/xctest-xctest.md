

- XCTest
-  XCTest 

Class

# XCTest

An abstract base class for creating, managing, and executing tests.

``` source
class XCTest
```

## Mentioned in 

Set Up and Tear Down State in Your Tests

## Overview

The XCTest class provides shared functionality that XCTestCase and XCTestSuite use for creating, managing, and executing tests. In most cases, you subclass XCTestCase directly when defining tests in your project.

## Topics

### Examining Test Properties

var name: String

The name of the test.

var testCaseCount: Int

The number of test cases in the test.

var testRun: XCTestRun?

The test run object that executes the test.

var testRunClass: AnyClass?

The test run subclass to instantiate when the test runs, which records the test’s results.

### Setting Up and Tearing Down

func setUp(completion: ((any Error)?) -> Void)

Provides an opportunity to reset state asynchronously and handle errors before calling each test method in a test case.

func setUpWithError() throws

Provides an opportunity to reset state and to throw errors before calling each test method in a test case.

func setUp()

Provides an opportunity to reset state before calling each test method in a test case.

func tearDown(completion: ((any Error)?) -> Void)

Provides an opportunity to perform cleanup asynchronously and handle errors after each test method in a test case ends.

func tearDownWithError() throws

Provides an opportunity to perform cleanup and to throw errors after each test method in a test case ends.

func tearDown()

Provides an opportunity to perform cleanup after each test method in a test case ends.

### Running Tests

func perform(XCTestRun)

Executes a specific test.

func run()

Creates a test run instance and starts the test.

## Relationships

### Inherits From

- NSObject

### Inherited By

- XCTestCase
- XCTestSuite

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Test cases and test methods

Defining Test Cases and Test Methods

Add test cases and test methods to a test target to confirm that your code performs as expected.

class XCTestCase

The primary class for defining test cases, test methods, and performance tests.

