

- XCTest
- XCTKeyPathExpectation
-  options 

Instance Property

# options

A combination of values that specify what to include in observation notifications.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+tvOS 13.0+

``` source
final let options: NSKeyValueObservingOptions
```

## Discussion

For possible values, see NSKeyValueObservingOptions.

## See Also

### Expectation properties

let keyPath: KeyPath&lt;T, V>

The key path for the observed property, relative to the observed object.

let observedObject: T

The object the system observes the key path on.

var expectedValue: V?

A value that the key path’s specified property must equal to fulfill the expectation.

