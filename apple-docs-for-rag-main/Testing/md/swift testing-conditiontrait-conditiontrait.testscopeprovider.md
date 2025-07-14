

- Swift Testing
- ConditionTrait
-  ConditionTrait.TestScopeProvider 

Type Alias

# ConditionTrait.TestScopeProvider

The type of the test scope provider for this trait.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
typealias TestScopeProvider = Never
```

## Discussion

The default type is `Never`, which cannot be instantiated. The `scopeProvider(for:testCase:)-cjmg` method for any trait with this default type must return `nil`, meaning that trait will not provide a custom scope for the tests it’s applied to.

