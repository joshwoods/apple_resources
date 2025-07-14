

- XCTest
- XCTKeyPathExpectation
-  init(keyPath:observedObject:options:predicate:) Deprecated

Initializer

# init(keyPath:observedObject:options:predicate:)

Creates an expectation that the system fulfills when the value of the observed property changes and satisfies the conditions of a predicate’s evaluation.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+tvOS 13.0+

``` source
convenience init(
    keyPath: KeyPath,
    observedObject: T,
    options: NSKeyValueObservingOptions = [.initial, .new, .old],
    predicate: XCTKeyPathExpectation.Predicate? = nil
)
```

Deprecated

T and V must be Sendable when used with an asynchronous filtering function.

## Parameters 

`keyPath`  

The key path for the observed property, relative to the observed object.

`observedObject`  

The object to observe the key path on.

`options`  

A combination of values that specify what to include in observation notifications. For possible values, see NSKeyValueObservingOptions.

`predicate`  

A closure that evaluates the value of the observed property. If `nil`, the first observed change fulfills the expectation.

## Discussion

Use this initializer to create an expectation that observes changes on the observed object until the predicate returns true, fulfilling the expectation.

## See Also

### Creating key path expectations

convenience init(keyPath: KeyPath&lt;T, V>, observedObject: T, options: NSKeyValueObservingOptions, expectedValue: V)

Creates an expectation that the system fulfills when the value of the observed property changes to an expected value.

convenience init(keyPath: KeyPath&lt;T, V>, observedObject: T, options: NSKeyValueObservingOptions, filter: XCTKeyPathExpectation&lt;T, V>.SynchronousFilter?)

convenience init(keyPath: KeyPath&lt;T, V>, observedObject: T, options: NSKeyValueObservingOptions, filter: XCTKeyPathExpectation&lt;T, V>.AsynchronousFilter?)

typealias AsynchronousFilter

typealias SynchronousFilter

typealias Predicate

A function the key path expectation uses to test the value of an observed property.

Deprecated

