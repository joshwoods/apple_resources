

- XCTest
- XCTKeyPathExpectation
-  init(keyPath:observedObject:options:filter:) 

Initializer

# init(keyPath:observedObject:options:filter:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+tvOS 13.0+

``` source
convenience init(
    keyPath: KeyPath,
    observedObject: T,
    options: NSKeyValueObservingOptions = [.initial, .new, .old],
    filter: XCTKeyPathExpectation.SynchronousFilter? = nil
)
```

Available when `T` inherits `NSObject`.

## See Also

### Creating key path expectations

convenience init(keyPath: KeyPath&lt;T, V>, observedObject: T, options: NSKeyValueObservingOptions, expectedValue: V)

Creates an expectation that the system fulfills when the value of the observed property changes to an expected value.

convenience init(keyPath: KeyPath&lt;T, V>, observedObject: T, options: NSKeyValueObservingOptions, predicate: XCTKeyPathExpectation&lt;T, V>.Predicate?)

Creates an expectation that the system fulfills when the value of the observed property changes and satisfies the conditions of a predicate’s evaluation.

Deprecated

convenience init(keyPath: KeyPath&lt;T, V>, observedObject: T, options: NSKeyValueObservingOptions, filter: XCTKeyPathExpectation&lt;T, V>.AsynchronousFilter?)

typealias AsynchronousFilter

typealias SynchronousFilter

typealias Predicate

A function the key path expectation uses to test the value of an observed property.

Deprecated

