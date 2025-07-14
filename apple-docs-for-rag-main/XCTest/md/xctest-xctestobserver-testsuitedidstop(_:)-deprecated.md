

- XCTest
- XCTestObserver
-  testSuiteDidStop(\_:) Deprecated

Instance Method

# testSuiteDidStop(\_:)

Notifies the observer when a test suite stops.

``` source
func testSuiteDidStop(_ testRun: XCTestRun!)
```

Deprecated

Use the XCTestObservationCenter class and XCTestObservation protocol instead.

## Parameters 

`testRun`  

The test run object calling this method.

## See Also

### Monitoring Test Activity

func testCaseDidFail(XCTestRun!, withDescription: String!, inFile: String!, atLine: Int)

Notifies the observer when a test case fails.

Deprecated

func testCaseDidStart(XCTestRun!)

Notifies the observer when a test case starts.

Deprecated

func testCaseDidStop(XCTestRun!)

Notifies the observer when a test case stops.

Deprecated

func testSuiteDidStart(XCTestRun!)

Notifies the observer when a test suite starts.

Deprecated

