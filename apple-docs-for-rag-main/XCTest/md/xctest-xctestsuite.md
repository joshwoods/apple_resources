

- XCTest
-  XCTestSuite 

Class

# XCTestSuite

A collection of test cases to manage as a test suite.

``` source
class XCTestSuite
```

## Overview

Typically, Xcode automatically manages test suites for you. Only use XCTestSuite if you need to define your own custom test suites programmatically.

## Topics

### Creating Test Suites

class var `default`: XCTestSuite

Creates a suite of test suites that represents all test case methods in the current runtime.

init(name: String)

Creates a test suite with the specified name.

convenience init(forBundlePath: String)

Creates a test suite with the bundle at the specified path.

convenience init(forTestCaseClass: AnyClass)

Creates a test suite that contains all test methods in the specified class.

convenience init(forTestCaseWithName: String)

Creates a test suite that contains a test case with the specified name.

### Managing Tests

func addTest(XCTest)

Adds a test to the test suite.

var tests: [XCTest]

All tests currently in the test suite.

## Relationships

### Inherits From

- XCTest

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

