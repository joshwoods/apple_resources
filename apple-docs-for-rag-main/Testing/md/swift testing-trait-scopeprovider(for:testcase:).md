

- Swift Testing
- Trait
-  scopeProvider(for:testCase:) 

Instance Method

# scopeProvider(for:testCase:)

Get this trait’s scope provider for the specified test and/or test case, if any.

Swift 6.1+Xcode 16.3+

``` source
func scopeProvider(
    for test: Test,
    testCase: Test.Case?
) -> Self.TestScopeProvider?
```

**Required** Default implementations provided.

## Parameters 

`test`  

The test for which a scope provider is being requested.

`testCase`  

The test case for which a scope provider is being requested, if any. When `test` represents a suite, the value of this argument is `nil`.

## Return Value

A value conforming to TestScopeProvider which may be used to provide custom scoping for `test` and/or `testCase`, or `nil` if they should not have any custom scope.

## Discussion

If this trait’s type conforms to TestScoping, the default value returned by this method depends on `test` and/or `testCase`:

- If `test` represents a suite, this trait must conform to SuiteTrait. If the value of this suite trait’s isRecursive property is `true`, then this method returns `nil`; otherwise, it returns `self`. This means that by default, a suite trait will *either* provide its custom scope once for the entire suite, or once per-test function it contains.

- Otherwise `test` represents a test function. If `testCase` is `nil`, this method returns `nil`; otherwise, it returns `self`. This means that by default, a trait which is applied to or inherited by a test function will provide its custom scope once for each of that function’s cases.

A trait may explicitly implement this method to further customize the default behaviors above. For example, if a trait should provide custom test scope both once per-suite and once per-test function in that suite, it may implement the method and return a non-`nil` scope provider under those conditions.

A trait may also implement this method and return `nil` if it determines that it does not need to provide a custom scope for a particular test at runtime, even if the test has the trait applied. This can improve performance and make diagnostics clearer by avoiding an unnecessary call to provideScope(for:testCase:performing:).

If this trait’s type does not conform to TestScoping and its associated TestScopeProvider type is the default `Never`, then this method returns `nil` by default. This means that instances of this trait will not provide a custom scope for tests to which they’re applied.

## Default Implementations

### Trait Implementations

func scopeProvider(for: Test, testCase: Test.Case?) -> Self?

Get this trait’s scope provider for the specified test and/or test case, if any.

func scopeProvider(for: Test, testCase: Test.Case?) -> Self?

Get this trait’s scope provider for the specified test and/or test case, if any.

func scopeProvider(for: Test, testCase: Test.Case?) -> Never?

Get this trait’s scope provider for the specified test and/or test case, if any.

## See Also

### Providing custom execution scope for tests

protocol TestScoping

A protocol that allows providing a custom execution scope for a test function (and each of its cases) or a test suite by performing custom code before or after it runs.

associatedtype TestScopeProvider : TestScoping = Never

The type of the test scope provider for this trait.

**Required**

