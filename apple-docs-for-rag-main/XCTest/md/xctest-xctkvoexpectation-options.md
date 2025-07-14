

- XCTest
- XCTKVOExpectation
-  options 

Instance Property

# options

The key-value observing options the expectation uses when registering for observation.

iOSiPadOSMac CatalystmacOSDeprecatedtvOSvisionOSDeprecatedwatchOSDeprecated

``` source
var options: NSKeyValueObservingOptions { get }
```

## See Also

### Expectation properties

var keyPath: String

The key path the system observes for KVO changes.

var observedObject: Any

The object that the system observes for KVO changes.

var expectedValue: Any?

The value that the key path’s specified property must equal to fulfill the expectation.

