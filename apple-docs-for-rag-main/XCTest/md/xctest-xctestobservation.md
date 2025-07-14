

- XCTest
-  XCTestObservation 

Protocol

# XCTestObservation

A protocol that defines methods the test runner calls in response to significant events during test runs.

``` source
protocol XCTestObservation : NSObjectProtocol
```

## Overview

The system calls the notification methods for XCTestObservation in the following sequence for a test bundle:

1.  testBundleWillStart(_:) — exactly once per test bundle

2.  testSuiteWillStart(_:) — exactly once per test suite

3.  testCaseWillStart(_:) — exactly once per test case

4.  testCase(_:didRecord:) — for each test failure, zero or more times per test case at any point between test case start and finish

5.  testCase(_:didRecord:) — for each expected test failure, zero or more times per test case at any point between test case start and finish

6.  testCaseDidFinish(_:) — exactly once per test case

7.  testSuite(_:didRecord:) — for each test failure, zero or more times per test suite at any point between test suite start and finish

8.  testSuite(_:didRecord:) — for each expected test failure, zero or more times per test suite at any point between test suite start and finish

9.  testSuiteDidFinish(_:) — exactly once per test suite

10. testBundleDidFinish(_:) — exactly once per test bundle

See XCTestObservationCenter for details about registering and removing test observers.

## Topics

### Observation Methods

func testBundleWillStart(Bundle)

Notifies the observer immediately before any tests in a test bundle begin.

func testSuiteWillStart(XCTestSuite)

Notifies the observer immediately before a test suite begins executing.

func testCaseWillStart(XCTestCase)

Notifies the observer immediately before a test case begins executing.

func testCase(XCTestCase, didRecord: XCTIssue)

Notifies the observer when a test case reports an issue.

func testCase(XCTestCase, didRecord: XCTExpectedFailure)

Notifies the observer when a test case records an expected failure.

func testCase(XCTestCase, didFailWithDescription: String, inFile: String?, atLine: Int)

Notifies the observer when a test case reports a failure.

Deprecated

func testCaseDidFinish(XCTestCase)

Notifies the observer immediately after a test case finishes executing.

func testSuite(XCTestSuite, didRecord: XCTIssue)

Notifies the observer when a test suite reports an issue.

func testSuite(XCTestSuite, didRecord: XCTExpectedFailure)

Notifies the observer when a test suite records an expected failure.

func testSuite(XCTestSuite, didFailWithDescription: String, inFile: String?, atLine: Int)

Notifies the observer when a test suite reports a failure.

Deprecated

func testSuiteDidFinish(XCTestSuite)

Notifies the observer immediately after a test suite finishes executing.

func testBundleDidFinish(Bundle)

Notifies the observer immediately after all tests in a test bundle finish executing.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Test Observation

class XCTestObservationCenter

Provides information about the progress of test runs to registered observers.

