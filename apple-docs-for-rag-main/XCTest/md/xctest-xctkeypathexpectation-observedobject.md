

- XCTest
- XCTKeyPathExpectation
-  observedObject 

Instance Property

# observedObject

The object the system observes the key path on.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+tvOS 13.0+

``` source
final let observedObject: T
```

## See Also

### Expectation properties

let keyPath: KeyPath&lt;T, V>

The key path for the observed property, relative to the observed object.

let options: NSKeyValueObservingOptions

A combination of values that specify what to include in observation notifications.

var expectedValue: V?

A value that the key path’s specified property must equal to fulfill the expectation.

