

- XCTest
- XCTNSPredicateExpectation
-  init(predicate:object:) 

Initializer

# init(predicate:object:)

Creates an expectation that’s fulfilled when an `NSPredicate` instance returns `true`, optionally for a provided object.

``` source
init(
    predicate: NSPredicate,
    object: Any?
)
```

## Parameters 

`predicate`  

The predicate to evaluate.

`object`  

An optional object XCTest evaluates the predicate against.

## Discussion

When you use an instance of this class from Swift and await using fulfillment(of:timeout:enforceOrder:) rather than wait(for:), XCTest evaluates `predicate` on the main actor.

