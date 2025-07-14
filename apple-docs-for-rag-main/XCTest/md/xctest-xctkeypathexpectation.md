

- XCTest
-  XCTKeyPathExpectation 

Class

# XCTKeyPathExpectation

An expectation that a specific key-value observing (KVO) condition fulfills.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+tvOS 13.0+

``` source
final class XCTKeyPathExpectation where T : NSObject
```

## Overview

Use an instance of this class to asynchronously wait for changes to a property you specify by key path for a given object. When the value of the property changes, the expectation compares the new value using a predicate or expected value you provide.

## Topics

### Creating key path expectations

convenience init(keyPath: KeyPath&lt;T, V>, observedObject: T, options: NSKeyValueObservingOptions, expectedValue: V)

Creates an expectation that the system fulfills when the value of the observed property changes to an expected value.

convenience init(keyPath: KeyPath&lt;T, V>, observedObject: T, options: NSKeyValueObservingOptions, predicate: XCTKeyPathExpectation&lt;T, V>.Predicate?)

Creates an expectation that the system fulfills when the value of the observed property changes and satisfies the conditions of a predicate’s evaluation.

Deprecated

convenience init(keyPath: KeyPath&lt;T, V>, observedObject: T, options: NSKeyValueObservingOptions, filter: XCTKeyPathExpectation&lt;T, V>.SynchronousFilter?)

convenience init(keyPath: KeyPath&lt;T, V>, observedObject: T, options: NSKeyValueObservingOptions, filter: XCTKeyPathExpectation&lt;T, V>.AsynchronousFilter?)

typealias AsynchronousFilter

typealias SynchronousFilter

typealias Predicate

A function the key path expectation uses to test the value of an observed property.

Deprecated

### Expectation properties

let keyPath: KeyPath&lt;T, V>

The key path for the observed property, relative to the observed object.

let observedObject: T

The object the system observes the key path on.

let options: NSKeyValueObservingOptions

A combination of values that specify what to include in observation notifications.

var expectedValue: V?

A value that the key path’s specified property must equal to fulfill the expectation.

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

### Related Documentation

Using Key-Value Observing in Swift

Notify objects about changes to the properties of other objects.

### Key Value Observing Expectations

class XCTKVOExpectation

An expectation that a specific key-value observing (KVO) condition fulfills.

