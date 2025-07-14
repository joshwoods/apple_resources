

- XCTest
- XCTestCase
-  expectation(description:) 

Instance Method

# expectation(description:)

Creates a new expectation with an associated description.

``` source
func expectation(description: String) -> XCTestExpectation
```

## Parameters 

`description`  

A string to display in the test log for this expectation, to help diagnose failures.

## Discussion

Use this method to create XCTestExpectation instances that can be fulfilled when asynchronous tasks in your tests complete.

To fulfill an expectation that was created with expectation(description:), call the expectation’s fulfill() method when the asynchronous task in your test has completed.

## See Also

### Creating Asynchronous Test Expectations

func expectation(for: NSPredicate, evaluatedWith: Any?, handler: XCTNSPredicateExpectation.Handler?) -> XCTestExpectation

Creates an expectation that the test fulfills by evaluating the predicate with the specified object.

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

