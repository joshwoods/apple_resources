

- XCTest
- XCTKVOExpectation
-  observedObject 

Instance Property

# observedObject

The object that the system observes for KVO changes.

iOSiPadOSMac CatalystmacOSDeprecatedtvOSvisionOSDeprecatedwatchOSDeprecated

``` source
var observedObject: Any { get }
```

## See Also

### Expectation properties

var keyPath: String

The key path the system observes for KVO changes.

var expectedValue: Any?

The value that the key path’s specified property must equal to fulfill the expectation.

var options: NSKeyValueObservingOptions

The key-value observing options the expectation uses when registering for observation.

