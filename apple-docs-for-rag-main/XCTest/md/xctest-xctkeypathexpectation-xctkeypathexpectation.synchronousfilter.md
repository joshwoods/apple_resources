

- XCTest
- XCTKeyPathExpectation
-  XCTKeyPathExpectation.SynchronousFilter 

Type Alias

# XCTKeyPathExpectation.SynchronousFilter

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+tvOS 13.0+

``` source
typealias SynchronousFilter = (T, NSKeyValueObservedChange) -> Bool
```

Available when `T` inherits `NSObject`.

## See Also

### Creating key path expectations

convenience init(keyPath: KeyPath&lt;T, V>, observedObject: T, options: NSKeyValueObservingOptions, expectedValue: V)

Creates an expectation that the system fulfills when the value of the observed property changes to an expected value.

convenience init(keyPath: KeyPath&lt;T, V>, observedObject: T, options: NSKeyValueObservingOptions, predicate: XCTKeyPathExpectation&lt;T, V>.Predicate?)

Creates an expectation that the system fulfills when the value of the observed property changes and satisfies the conditions of a predicate’s evaluation.

Deprecated

convenience init(keyPath: KeyPath&lt;T, V>, observedObject: T, options: NSKeyValueObservingOptions, filter: XCTKeyPathExpectation&lt;T, V>.SynchronousFilter?)

convenience init(keyPath: KeyPath&lt;T, V>, observedObject: T, options: NSKeyValueObservingOptions, filter: XCTKeyPathExpectation&lt;T, V>.AsynchronousFilter?)

typealias AsynchronousFilter

typealias Predicate

A function the key path expectation uses to test the value of an observed property.

Deprecated

