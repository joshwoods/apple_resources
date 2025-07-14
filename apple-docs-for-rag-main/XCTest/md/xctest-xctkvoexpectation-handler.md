

- XCTest
- XCTKVOExpectation
-  handler 

Instance Property

# handler

An optional handler that performs custom evaluation of changes to the observed key path.

iOSiPadOSMac CatalystmacOSDeprecatedtvOSvisionOSDeprecatedwatchOSDeprecated

``` source
var handler: XCTKVOExpectation.Handler? { get set }
```

## Discussion

Note

The system ignores the expectation’s expectedValue property when the handler is non-nil.

## See Also

### Custom KVO evaluation

typealias Handler

A custom handler to call when observing a KVO change for a specified key path.

