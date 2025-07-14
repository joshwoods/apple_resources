

- Swift Testing
- Bug
-  scopeProvider(for:testCase:) 

Instance Method

# scopeProvider(for:testCase:)

Get this trait’s scope provider for the specified test and/or test case, if any.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
func scopeProvider(
    for test: Test,
    testCase: Test.Case?
) -> Never?
```

Available when `TestScopeProvider` is `Never`.

## Parameters 

`test`  

The test for which a scope provider is being requested.

`testCase`  

The test case for which a scope provider is being requested, if any. When `test` represents a suite, the value of this argument is `nil`.

## Discussion

This default implementation is used when this trait type’s associated TestScopeProvider type is the default value of `Never`, and its return value is discussed in scopeProvider(for:testCase:).

