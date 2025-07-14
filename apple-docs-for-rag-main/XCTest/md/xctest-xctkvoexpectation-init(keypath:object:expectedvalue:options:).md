

- XCTest
- XCTKVOExpectation
-  init(keyPath:object:expectedValue:options:) 

Initializer

# init(keyPath:object:expectedValue:options:)

Creates an expectation with custom observation options that a KVO change fulfills when it causes the specified key path of the observed object to have an expected value.

iOSiPadOSMac CatalystmacOSDeprecatedtvOSvisionOSDeprecatedwatchOSDeprecated

``` source
init(
    keyPath: String,
    object: Any,
    expectedValue: Any?,
    options: NSKeyValueObservingOptions = []
)
```

## Parameters 

`keyPath`  

The key path to observe.

`object`  

The object to observe.

`expectedValue`  

The expected value for the observed key path.

`options`  

An array of NSKeyValueObservingOptions that determine the values to return as part of the observed key path’s change dictionary.

## See Also

### Creating KVO expectations

convenience init(keyPath: String, object: Any)

Creates an expectation that any KVO change to the specified key path of the observed object fulfills.

convenience init(keyPath: String, object: Any, expectedValue: Any?)

Creates an expectation a KVO change fulfills when it causes the specified key path of the observed object to have an expected value.

