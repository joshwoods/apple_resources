

- XCTest
-  XCTestCaseRun 

Class

# XCTestCaseRun

An object that collects information about a specific execution of a test case.

``` source
class XCTestCaseRun
```

## Overview

The test runner manages the creation and tracking of `XCTestCaseRun` for each XCTestCase in an XCTestSuite.

## Topics

### Deprecated

func recordFailure(inTest: XCTestCase, withDescription: String, inFile: String, atLine: Int, expected: Bool)

Records a test failure during test execution for this test run.

Deprecated

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

class XCTestSuiteRun

An object that collects information about a specific execution of a test suite.

class XCTestRun

A base class for collecting information about a specific execution of a test.

