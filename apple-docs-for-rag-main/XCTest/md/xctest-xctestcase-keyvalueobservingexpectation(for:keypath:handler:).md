

- XCTest
- XCTestCase
-  keyValueObservingExpectation(for:keyPath:handler:) 

Instance Method

# keyValueObservingExpectation(for:keyPath:handler:)

Creates an expectation that uses Key-Value Observing to observe a value and respond to changes in that value by calling a provided handler.

iOSiPadOSMac CatalystmacOSDeprecatedtvOSvisionOSDeprecatedwatchOSDeprecated

``` source
func keyValueObservingExpectation(
    for objectToObserve: Any,
    keyPath: String,
    handler: XCTKVOExpectation.Handler? = nil
) -> XCTestExpectation
```

## Parameters 

`objectToObserve`  

The object to observe.

`keyPath`  

The key path to observe.

`handler`  

An optional XCTKVOExpectation.Handler block. If you don’t provide a handler block, the first change to the key path of the observed object fulfills the expectation.

## Discussion

Creates an XCTestExpectation that uses Key Value Observing to observe changes on the value specified by `keyPath` on the provided object.

When the tests detects changes to the value, it calls the `handler` block to assess the new value to see if the change fulfills the expectation. Every key-value observing change runs the handler block until it either returns true (to fulfill the expectation), or the wait times out.

You can use XCTAssert and related APIs in the block to report a failure.

Note

For more control over KVO-based expectations, use XCTKVOExpectation instead of this convenience method.

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

func expectation&lt;T, V>(that: KeyPath&lt;T, V>, on: T, options: NSKeyValueObservingOptions, willEqual: V) -> XCTKeyPathExpectation&lt;T, V>

Creates an expectation using key-value observing the test fulfills when the value of an observed property changes to an expected value.

func expectation&lt;T, V>(that: KeyPath&lt;T, V>, on: T, options: NSKeyValueObservingOptions, willSatisfy: XCTKeyPathExpectation&lt;T, V>.Predicate?) -> XCTKeyPathExpectation&lt;T, V>

Creates an expectation using key-value observing the test fulfills when the value of an observed property changes and satisfies the conditions of a predicate’s evaluation.

Deprecated

func expectation&lt;T, V>(that: KeyPath&lt;T, V>, on: T, options: NSKeyValueObservingOptions, willSatisfy: XCTKeyPathExpectation&lt;T, V>.AsynchronousFilter?) -> XCTKeyPathExpectation&lt;T, V>

Creates an expectation using key-value observing to monitor changes to a given key path on a given object.

func expectation&lt;T, V>(that: KeyPath&lt;T, V>, on: T, options: NSKeyValueObservingOptions, willSatisfy: XCTKeyPathExpectation&lt;T, V>.SynchronousFilter?) -> XCTKeyPathExpectation&lt;T, V>

Creates an expectation using key-value observing to monitor changes to a given key path on a given object.

