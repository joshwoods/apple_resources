

- XCTest
- XCTestObserver
-  testSuiteDidStart(\_:) Deprecated

Instance Method

# testSuiteDidStart(\_:)

Notifies the observer when a test suite starts.

``` source
func testSuiteDidStart(_ testRun: XCTestRun!)
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

func testCaseDidStop(XCTestRun!)

Notifies the observer when a test case stops.

Deprecated

func testSuiteDidStop(XCTestRun!)

Notifies the observer when a test suite stops.

Deprecated

