

- XCTest
- XCTestObservation
-  testSuite(\_:didRecord:) 

Instance Method

# testSuite(\_:didRecord:)

Notifies the observer when a test suite reports an issue.

**macOS**

``` source
optional func testSuite(
    _ testSuite: XCTestSuite,
    didRecord issue: XCTIssueReference
)
```

**iOS, iPadOS, tvOS, visionOS, watchOS**

``` source
optional func testSuite(
    _ testSuite: XCTestSuite,
    didRecord issue: XCTIssue
)
```

## Parameters 

`testSuite`  

The test suite with the issue.

`issue`  

The issue to record.

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

func testSuite(XCTestSuite, didRecord: XCTExpectedFailure)

Notifies the observer when a test suite records an expected failure.

func testSuite(XCTestSuite, didFailWithDescription: String, inFile: String?, atLine: Int)

Notifies the observer when a test suite reports a failure.

Deprecated

func testSuiteDidFinish(XCTestSuite)

Notifies the observer immediately after a test suite finishes executing.

func testBundleDidFinish(Bundle)

Notifies the observer immediately after all tests in a test bundle finish executing.

