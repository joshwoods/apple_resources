

- XCTest
-  XCTestObservationCenter 

Class

# XCTestObservationCenter

Provides information about the progress of test runs to registered observers.

``` source
class XCTestObservationCenter
```

## Overview

Observers can be any object that conforms to the XCTestObservation protocol. Register new observers with the addTestObserver(_:) method and remove them with the removeTestObserver(_:) method.

If an NSPrincipalClass key is declared in the test bundle’s Info.plist file, XCTest automatically creates a single instance of that class when the test bundle is loaded. You can use this instance as a place to register observers or do other pretesting global setup before testing for that bundle begins.

Important

Observers must be registered manually. The NSPrincipalClass instance is not automatically registered as an observer even if the class conforms to XCTestObservation.

## Topics

### Accessing the Shared Observation Center

class var shared: XCTestObservationCenter

The shared XCTestObservationCenter singleton instance.

### Managing Observers

func addTestObserver(any XCTestObservation)

Registers an object conforming to XCTestObservation as an observer for the current test session.

func removeTestObserver(any XCTestObservation)

Unregisters an object conforming to XCTestObservation as an observer for the current test session.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Test Observation

protocol XCTestObservation

A protocol that defines methods the test runner calls in response to significant events during test runs.

