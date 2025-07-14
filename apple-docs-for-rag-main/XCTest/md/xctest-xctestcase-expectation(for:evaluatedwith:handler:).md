

- XCTest
- XCTestCase
-  expectation(for:evaluatedWith:handler:) 

Instance Method

# expectation(for:evaluatedWith:handler:)

Creates an expectation that the test fulfills by evaluating the predicate with the specified object.

``` source
func expectation(
    for predicate: NSPredicate,
    evaluatedWith object: Any?,
    handler: XCTNSPredicateExpectation.Handler? = nil
) -> XCTestExpectation
```

## Parameters 

`predicate`  

The predicate to evaluate.

`object`  

The object XCTest evaluates the predicate against.

`handler`  

An optional handler that performs custom evaluation when `predicate` evaluates as true.

## Discussion

The expectation periodically evaluates the predicate and also may use notifications or other events to optimistically re-evaluate. The test fulfills the expectation when the predicate evaluates to true.

When you use the resulting expectation from Swift and await using fulfillment(of:timeout:enforceOrder:) rather than wait(for:), XCTest evaluates `predicate` on the main actor.

If a handler isn’t provided, the first successful evaluation of the predicate fulfills the expectation. If you provide a handler, the handler can override this default behavior to tailor the conditions that fulfill the expectation.

Note

For more control over predicate-based expectations, use XCTNSPredicateExpectation instead of this convenience method.

## See Also

### Creating Asynchronous Test Expectations

func expectation(description: String) -> XCTestExpectation

Creates a new expectation with an associated description.

func expectation(forNotification: NSNotification.Name, object: Any?, handler: XCTNSNotificationExpectation.Handler?) -> XCTestExpectation

Creates an expectation that the test fulfills when it receives a specific notification for a specified object.

func expectation(forNotification: NSNotification.Name, object: Any?, notificationCenter: NotificationCenter, handler: XCTNSNotificationExpectation.Handler?) -> XCTestExpectation

Creates an expectation that the test fulfills when it receives a specific notification from a specific notification center for a specified object.

func keyValueObservingExpectation(for: Any, keyPath: String, expectedValue: Any?) -> XCTestExpectation

Creates an expectation that uses Key-Value Observing to observe a value until it matches an expected value.

func expectation&lt;T, V>(that: KeyPath&lt;T, V>, on: T, options: NSKeyValueObservingOptions, willEqual: V) -> XCTKeyPathExpectation&lt;T, V>

Creates an expectation using key-value observing the test fulfills when the value of an observed property changes to an expected value.

func keyValueObservingExpectation(for: Any, keyPath: String, handler: XCTKVOExpectation.Handler?) -> XCTestExpectation

Creates an expectation that uses Key-Value Observing to observe a value and respond to changes in that value by calling a provided handler.

func expectation&lt;T, V>(that: KeyPath&lt;T, V>, on: T, options: NSKeyValueObservingOptions, willSatisfy: XCTKeyPathExpectation&lt;T, V>.Predicate?) -> XCTKeyPathExpectation&lt;T, V>

Creates an expectation using key-value observing the test fulfills when the value of an observed property changes and satisfies the conditions of a predicate’s evaluation.

Deprecated

func expectation&lt;T, V>(that: KeyPath&lt;T, V>, on: T, options: NSKeyValueObservingOptions, willSatisfy: XCTKeyPathExpectation&lt;T, V>.AsynchronousFilter?) -> XCTKeyPathExpectation&lt;T, V>

Creates an expectation using key-value observing to monitor changes to a given key path on a given object.

func expectation&lt;T, V>(that: KeyPath&lt;T, V>, on: T, options: NSKeyValueObservingOptions, willSatisfy: XCTKeyPathExpectation&lt;T, V>.SynchronousFilter?) -> XCTKeyPathExpectation&lt;T, V>

Creates an expectation using key-value observing to monitor changes to a given key path on a given object.

