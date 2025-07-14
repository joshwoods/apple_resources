

- XCTest
- XCTestObservation
-  testSuite(\_:didFailWithDescription:inFile:atLine:) Deprecated

Instance Method

# testSuite(\_:didFailWithDescription:inFile:atLine:)

Notifies the observer when a test suite reports a failure.

``` source
optional func testSuite(
    _ testSuite: XCTestSuite,
    didFailWithDescription description: String,
    inFile filePath: String?,
    atLine lineNumber: Int
)
```

Deprecated

Use testSuite(_:didRecord:) instead. If you implement both this method and testSuite(_:didRecord:), the test will not call this method.

## Parameters 

`testSuite`  

The test suite that failed. Additional information about the suite can be retrieved from the test suite’s associated XCTestRun.

`description`  

A textual description of the failure.

`filePath`  

The path to the file in the failure occurred, or `nil` if the file path is unknown.

`lineNumber`  

The line number on which the failure was reported.

## Discussion

Suite failures are most commonly reported during suite-level setup and teardown. Failures during tests are reported for the test case alone and are not reported as suite failures.

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

func testSuiteDidFinish(XCTestSuite)

Notifies the observer immediately after a test suite finishes executing.

func testBundleDidFinish(Bundle)

Notifies the observer immediately after all tests in a test bundle finish executing.

