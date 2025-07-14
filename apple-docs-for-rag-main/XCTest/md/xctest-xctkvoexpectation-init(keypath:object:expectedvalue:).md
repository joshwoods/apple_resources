

- XCTest
- XCTKVOExpectation
-  init(keyPath:object:expectedValue:) 

Initializer

# init(keyPath:object:expectedValue:)

Creates an expectation a KVO change fulfills when it causes the specified key path of the observed object to have an expected value.

iOSiPadOSMac CatalystmacOSDeprecatedtvOSvisionOSDeprecatedwatchOSDeprecated

``` source
convenience init(
    keyPath: String,
    object: Any,
    expectedValue: Any?
)
```

## Parameters 

`keyPath`  

The key path to observe.

`object`  

The object to observe.

`expectedValue`  

The expected value for the observed key path.

## Discussion

This initializer sets up KVO observation for `keyPath` with the following NSKeyValueObservingOptions:

- initial

- new

- old

The inclusion of the initial option means that the system checks the observed key path immediately after initialization. The inclusion of the new and old options means that any custom KVO handler you provide in the expectation’s handler property receives a change info dictionary that contains the newKey and oldKey keys.

## See Also

### Creating KVO expectations

convenience init(keyPath: String, object: Any)

Creates an expectation that any KVO change to the specified key path of the observed object fulfills.

init(keyPath: String, object: Any, expectedValue: Any?, options: NSKeyValueObservingOptions)

Creates an expectation with custom observation options that a KVO change fulfills when it causes the specified key path of the observed object to have an expected value.

