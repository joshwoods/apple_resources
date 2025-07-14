

- XCTest
- XCTestObservation
-  testBundleDidFinish(\_:) 

Instance Method

# testBundleDidFinish(\_:)

Notifies the observer immediately after all tests in a test bundle finish executing.

``` source
optional func testBundleDidFinish(_ testBundle: Bundle)
```

## Parameters 

`testBundle`  

The bundle containing the tests that were executed.

## Discussion

This method provides a customization point for any post-testing activity. The test process will generally exit after this method returns, so if there is long running and/or asynchronous work to be done after testing, be sure to implement this method in a way that blocks until all long running activity is complete.

## See Also

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

