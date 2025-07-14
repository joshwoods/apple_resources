

- XCTest
- XCTestObserver
-  testCaseDidFail(\_:withDescription:inFile:atLine:) Deprecated

Instance Method

# testCaseDidFail(\_:withDescription:inFile:atLine:)

Notifies the observer when a test case fails.

``` source
func testCaseDidFail(
    _ testRun: XCTestRun!,
    withDescription description: String!,
    inFile filePath: String!,
    atLine lineNumber: Int
)
```

Deprecated

Use the XCTestObservationCenter class and XCTestObservation protocol instead.

## Parameters 

`testRun`  

The test run object that calls this method.

`description`  

A string description of the failed test.

`filePath`  

A string that represents a file path to a source code file when the test encounters a failure.

`lineNumber`  

An integer value that represents the line number in the source code file when the test encounters a failure.

## See Also

### Monitoring Test Activity

func testCaseDidStart(XCTestRun!)

Notifies the observer when a test case starts.

Deprecated

func testCaseDidStop(XCTestRun!)

Notifies the observer when a test case stops.

Deprecated

func testSuiteDidStart(XCTestRun!)

Notifies the observer when a test suite starts.

Deprecated

func testSuiteDidStop(XCTestRun!)

Notifies the observer when a test suite stops.

Deprecated

