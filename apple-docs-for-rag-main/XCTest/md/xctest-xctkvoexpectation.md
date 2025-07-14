

- XCTest
-  XCTKVOExpectation 

Class

# XCTKVOExpectation

An expectation that a specific key-value observing (KVO) condition fulfills.

iOSiPadOSMac CatalystmacOSDeprecatedtvOSvisionOSDeprecatedwatchOSDeprecated

``` source
class XCTKVOExpectation
```

## Overview

Apple discourages the use of this symbol in Swift. Use XCTKeyPathExpectation instead.

## Topics

### Creating KVO expectations

convenience init(keyPath: String, object: Any)

Creates an expectation that any KVO change to the specified key path of the observed object fulfills.

convenience init(keyPath: String, object: Any, expectedValue: Any?)

Creates an expectation a KVO change fulfills when it causes the specified key path of the observed object to have an expected value.

init(keyPath: String, object: Any, expectedValue: Any?, options: NSKeyValueObservingOptions)

Creates an expectation with custom observation options that a KVO change fulfills when it causes the specified key path of the observed object to have an expected value.

### Expectation properties

var keyPath: String

The key path the system observes for KVO changes.

var observedObject: Any

The object that the system observes for KVO changes.

var expectedValue: Any?

The value that the key path’s specified property must equal to fulfill the expectation.

var options: NSKeyValueObservingOptions

The key-value observing options the expectation uses when registering for observation.

### Custom KVO evaluation

var handler: XCTKVOExpectation.Handler?

An optional handler that performs custom evaluation of changes to the observed key path.

typealias Handler

A custom handler to call when observing a KVO change for a specified key path.

## Relationships

### Inherits From

- XCTestExpectation

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Key Value Observing Expectations

class XCTKeyPathExpectation

An expectation that a specific key-value observing (KVO) condition fulfills.

