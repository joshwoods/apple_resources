

- XCTest
- XCTestObserver
-  testCaseDidStop(\_:) Deprecated

Instance Method

# testCaseDidStop(\_:)

Notifies the observer when a test case stops.

``` source
func testCaseDidStop(_ testRun: XCTestRun!)
```

Deprecated

Use the XCTestObservationCenter class and XCTestObservation protocol instead.

## Parameters 

`testRun`  

The test run object that calls this method.

## See Also

### Monitoring Test Activity

func testCaseDidFail(XCTestRun!, withDescription: String!, inFile: String!, atLine: Int)

Notifies the observer when a test case fails.

Deprecated

func testCaseDidStart(XCTestRun!)

Notifies the observer when a test case starts.

Deprecated

func testSuiteDidStart(XCTestRun!)

Notifies the observer when a test suite starts.

Deprecated

func testSuiteDidStop(XCTestRun!)

Notifies the observer when a test suite stops.

Deprecated

