

- Swift Testing
- Trait
-  TestScopeProvider 

Associated Type

# TestScopeProvider

The type of the test scope provider for this trait.

Swift 6.1+Xcode 16.3+

``` source
associatedtype TestScopeProvider : TestScoping = Never
```

**Required**

## Discussion

The default type is `Never`, which cannot be instantiated. The scopeProvider(for:testCase:) method for any trait with this default type must return `nil`, meaning that trait will not provide a custom scope for the tests it’s applied to.

## See Also

### Providing custom execution scope for tests

protocol TestScoping

A protocol that allows providing a custom execution scope for a test function (and each of its cases) or a test suite by performing custom code before or after it runs.

func scopeProvider(for: Test, testCase: Test.Case?) -> Self.TestScopeProvider?

Get this trait’s scope provider for the specified test and/or test case, if any.

**Required** Default implementations provided.

