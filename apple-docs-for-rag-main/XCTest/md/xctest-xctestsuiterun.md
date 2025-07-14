

- XCTest
-  XCTestSuiteRun 

Class

# XCTestSuiteRun

An object that collects information about a specific execution of a test suite.

``` source
class XCTestSuiteRun
```

## Overview

The test runner manages the creation and tracking of `XCTestSuiteRun` for an XCTestSuite.

## Topics

### Managing Test Runs

func addTestRun(XCTestRun)

Adds a test run to the test suite.

var testRuns: [XCTestRun]

An array of test runs that the test suite manages.

## Relationships

### Inherits From

- XCTestRun

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Test Runs

class XCTestCaseRun

An object that collects information about a specific execution of a test case.

class XCTestRun

A base class for collecting information about a specific execution of a test.

