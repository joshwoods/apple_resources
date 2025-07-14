

- XCTest
- XCTestCase
-  expectation(that:on:options:willEqual:) 

Instance Method

# expectation(that:on:options:willEqual:)

Creates an expectation using key-value observing the test fulfills when the value of an observed property changes to an expected value.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+tvOS 13.0+

``` source
func expectation(
    that keyPath: KeyPath,
    on observedObject: T,
    options: NSKeyValueObservingOptions = [.initial, .new, .old],
    willEqual expectedValue: V
) -> XCTKeyPathExpectation where T : NSObject, V : Equatable
```

## Parameters 

`keyPath`  

The key path for the observed property, relative to the observed object.

`observedObject`  

The object to observe the key path on.

`options`  

A combination of values that specify what to include in observation notifications. For possible values, see NSKeyValueObservingOptions.

`expectedValue`  

A value the property must equal to fulfill the expectation.

## Return Value

Creates and returns an expectation for the test case.

## See Also

### Creating Asynchronous Test Expectations

func expectation(description: String) -> XCTestExpectation

Creates a new expectation with an associated description.

func expectation(for: NSPredicate, evaluatedWith: Any?, handler: XCTNSPredicateExpectation.Handler?) -> XCTestExpectation

Creates an expectation that the test fulfills by evaluating the predicate with the specified object.

func expectation(forNotification: NSNotification.Name, object: Any?, handler: XCTNSNotificationExpectation.Handler?) -> XCTestExpectation

Creates an expectation that the test fulfills when it receives a specific notification for a specified object.

func expectation(forNotification: NSNotification.Name, object: Any?, notificationCenter: NotificationCenter, handler: XCTNSNotificationExpectation.Handler?) -> XCTestExpectation

Creates an expectation that the test fulfills when it receives a specific notification from a specific notification center for a specified object.

func keyValueObservingExpectation(for: Any, keyPath: String, expectedValue: Any?) -> XCTestExpectation

Creates an expectation that uses Key-Value Observing to observe a value until it matches an expected value.

func keyValueObservingExpectation(for: Any, keyPath: String, handler: XCTKVOExpectation.Handler?) -> XCTestExpectation

Creates an expectation that uses Key-Value Observing to observe a value and respond to changes in that value by calling a provided handler.

func expectation&lt;T, V>(that: KeyPath&lt;T, V>, on: T, options: NSKeyValueObservingOptions, willSatisfy: XCTKeyPathExpectation&lt;T, V>.Predicate?) -> XCTKeyPathExpectation&lt;T, V>

Creates an expectation using key-value observing the test fulfills when the value of an observed property changes and satisfies the conditions of a predicate’s evaluation.

Deprecated

func expectation&lt;T, V>(that: KeyPath&lt;T, V>, on: T, options: NSKeyValueObservingOptions, willSatisfy: XCTKeyPathExpectation&lt;T, V>.AsynchronousFilter?) -> XCTKeyPathExpectation&lt;T, V>

Creates an expectation using key-value observing to monitor changes to a given key path on a given object.

func expectation&lt;T, V>(that: KeyPath&lt;T, V>, on: T, options: NSKeyValueObservingOptions, willSatisfy: XCTKeyPathExpectation&lt;T, V>.SynchronousFilter?) -> XCTKeyPathExpectation&lt;T, V>

Creates an expectation using key-value observing to monitor changes to a given key path on a given object.

