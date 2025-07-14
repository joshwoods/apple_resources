

- XCTest
- XCTestCase
-  expectation(forNotification:object:handler:) 

Instance Method

# expectation(forNotification:object:handler:)

Creates an expectation that the test fulfills when it receives a specific notification for a specified object.

``` source
func expectation(
    forNotification notificationName: NSNotification.Name,
    object objectToObserve: Any?,
    handler: XCTNSNotificationExpectation.Handler? = nil
) -> XCTestExpectation
```

## Parameters 

`notificationName`  

The notification to register for.

`objectToObserve`  

The object to observe.

`handler`  

An optional XCTNSNotificationExpectation.Handler block. If no handler is provided, the first notification matching the specified name from the observed object fulfills the expectation.

## Discussion

Note

For more control over notification-based expectations, use XCTNSNotificationExpectation instead of this convenience method.

## See Also

### Creating Asynchronous Test Expectations

func expectation(description: String) -> XCTestExpectation

Creates a new expectation with an associated description.

func expectation(for: NSPredicate, evaluatedWith: Any?, handler: XCTNSPredicateExpectation.Handler?) -> XCTestExpectation

Creates an expectation that the test fulfills by evaluating the predicate with the specified object.

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

