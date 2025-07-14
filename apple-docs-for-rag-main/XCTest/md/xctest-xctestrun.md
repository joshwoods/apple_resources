

- XCTest
-  XCTestRun 

Class

# XCTestRun

A base class for collecting information about a specific execution of a test.

``` source
class XCTestRun
```

## Overview

`XCTestRun` classifies failures in explicit test assertions as *expected*, and failures from unrelated or uncaught exceptions as *unexpected*.

## Topics

### Creating Test Runs

init(test: XCTest)

Creates a new test run for the provided test.

### Performing Test Runs

func start()

Starts a test run.

func stop()

Stops a test run.

func record(XCTIssue)

Records an issue during test execution for the test run.

### Tracking Test Durations

var startDate: Date?

The date and time when the test run started, or no value if the test hasn’t run.

var stopDate: Date?

The date and time when the test run stopped, or no value if the test hasn’t run.

var testDuration: TimeInterval

The number of seconds that elapse between when the run starts and when it stops.

var totalDuration: TimeInterval

The number of seconds that elapse between when the run starts and when it stops.

### Gathering Test Outcomes

var hasSucceeded: Bool

A Boolean value that returns true if all tests in the run completed without recording any failures; otherwise, false.

var hasBeenSkipped: Bool

A Boolean value that indicates a skipped test.

var executionCount: Int

The number of test executions during the run.

var failureCount: Int

The number of test failures during the run.

var skipCount: Int

The number of skipped tests during the run.

var test: XCTest

The test instance for the test run.

var testCaseCount: Int

The number of tests in the run.

var totalFailureCount: Int

The number of test failures and uncaught exceptions during the run.

var unexpectedExceptionCount: Int

The number of uncaught exceptions during the run.

### Deprecated

func recordFailure(withDescription: String, inFile: String?, atLine: Int, expected: Bool)

Records a failure during test execution for the test run.

Deprecated

## Relationships

### Inherits From

- NSObject

### Inherited By

- XCTestCaseRun
- XCTestSuiteRun

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

class XCTestSuiteRun

An object that collects information about a specific execution of a test suite.

