

- XCTest
- XCTKeyPathExpectation
-  expectedValue 

Instance Property

# expectedValue

A value that the key path’s specified property must equal to fulfill the expectation.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+tvOS 13.0+

``` source
final var expectedValue: V? { get }
```

Available when `T` inherits `NSObject` and `V` conforms to `Equatable`.

## Discussion

If the expectation doesn’t initialize with an expected value, this property returns `nil`.

## See Also

### Expectation properties

let keyPath: KeyPath&lt;T, V>

The key path for the observed property, relative to the observed object.

let observedObject: T

The object the system observes the key path on.

let options: NSKeyValueObservingOptions

A combination of values that specify what to include in observation notifications.

