

- Swift Testing
- TimeLimitTrait
-  TimeLimitTrait.TestScopeProvider 

Type Alias

# TimeLimitTrait.TestScopeProvider

The type of the test scope provider for this trait.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+Swift 6.0+Xcode 16.0+

``` source
typealias TestScopeProvider = Never
```

## Discussion

The default type is `Never`, which cannot be instantiated. The `scopeProvider(for:testCase:)-cjmg` method for any trait with this default type must return `nil`, meaning that trait will not provide a custom scope for the tests it’s applied to.

