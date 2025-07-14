

- XCTest
- XCTestObservation
-  testCaseWillStart(\_:) 

Instance Method

# testCaseWillStart(\_:)

Notifies the observer immediately before a test case begins executing.

``` source
optional func testCaseWillStart(_ testCase: XCTestCase)
```

## Parameters 

`testCase`  

The test case that is about to start. Additional information about the test case can be retrieved from the test case’s associated XCTestRun.

## See Also

### Observation Methods

func testBundleWillStart(Bundle)

Notifies the observer immediately before any tests in a test bundle begin.

func testSuiteWillStart(XCTestSuite)

Notifies the observer immediately before a test suite begins executing.

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

