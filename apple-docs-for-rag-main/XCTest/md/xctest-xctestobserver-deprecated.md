

- XCTest
-  XCTestObserver Deprecated

Class

# XCTestObserver

An object that observes test activity and events.

``` source
class XCTestObserver
```

Deprecated

Use XCTestObservationCenter instead.

## Topics

### Starting and Stopping Test Observation

func startObserving()

Starts observing a test.

func stopObserving()

Stops observing a test.

### Monitoring Test Activity

func testCaseDidFail(XCTestRun!, withDescription: String!, inFile: String!, atLine: Int)

Notifies the observer when a test case fails.

func testCaseDidStart(XCTestRun!)

Notifies the observer when a test case starts.

func testCaseDidStop(XCTestRun!)

Notifies the observer when a test case stops.

func testSuiteDidStart(XCTestRun!)

Notifies the observer when a test suite starts.

func testSuiteDidStop(XCTestRun!)

Notifies the observer when a test suite stops.

## Relationships

### Inherits From

- NSObject

### Inherited By

- XCTestLog

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Deprecated Classes

class XCTestLog

An object that logs test failures and errors.

Deprecated

class XCTestProbe

An object that observes test activity status.

Deprecated

