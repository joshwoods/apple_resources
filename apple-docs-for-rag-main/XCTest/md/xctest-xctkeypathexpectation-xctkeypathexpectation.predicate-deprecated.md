

- XCTest
- XCTKeyPathExpectation
-  XCTKeyPathExpectation.Predicate Deprecated

Type Alias

# XCTKeyPathExpectation.Predicate

A function the key path expectation uses to test the value of an observed property.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+tvOS 13.0+

``` source
typealias Predicate = (T, NSKeyValueObservedChange) async -> Bool
```

Deprecated

T and V must be Sendable when used with an asynchronous filtering function.

## Parameters 

`observedObject`  

The observed object to evaluate with the property that changes.

`change`  

A value that describes the observed change.

## Return Value

Returns true if the change fulfills the expectation; otherwise, false.

## Discussion

A key path expectation uses this function to determine whether the value of the observed property fulfills the conditions of the expectation. The system invokes the function asyncronously on a detached task and may call the function more that once.

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

typealias SynchronousFilter

