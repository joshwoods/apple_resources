

- XCTest
- XCTKeyPathExpectation
-  keyPath 

Instance Property

# keyPath

The key path for the observed property, relative to the observed object.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+tvOS 13.0+

``` source
final let keyPath: KeyPath
```

## See Also

### Expectation properties

let observedObject: T

The object the system observes the key path on.

let options: NSKeyValueObservingOptions

A combination of values that specify what to include in observation notifications.

var expectedValue: V?

A value that the key path’s specified property must equal to fulfill the expectation.

