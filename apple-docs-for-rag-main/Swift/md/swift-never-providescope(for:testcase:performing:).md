

- Swift
- Never
-  provideScope(for:testCase:performing:) 

Instance Method

# provideScope(for:testCase:performing:)

Provide custom execution scope for a function call which is related to the specified test or test case.

iOS 8.0+iPadOS 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func provideScope(
    for test: Test,
    testCase: Test.Case?,
    performing function: () async throws -> Void
) async throws
```

## Parameters 

`test`  

The test which `function` encapsulates.

`testCase`  

The test case, if any, which `function` encapsulates. When invoked on a suite, the value of this argument is `nil`.

`function`  

The function to perform. If `test` represents a test suite, this function encapsulates running all the tests in that suite. If `test` represents a test function, this function is the body of that test function (including all cases if the test function is parameterized.)

## Discussion

Throws

Any error that `function` throws, or an error that prevents this type from providing a custom scope correctly. The testing library records an error thrown from this method as an issue associated with `test`. If an error is thrown before this method calls `function`, the corresponding test doesn’t run.

When the testing library prepares to run a test, it starts by finding all traits applied to that test, including those inherited from containing suites. It begins with inherited suite traits, sorting them outermost-to-innermost, and if the test is a function, it then adds all traits applied directly to that functions in the order they were applied (left-to-right). It then asks each trait for its scope provider (if any) by calling `Trait/scopeProvider(for:testCase:)-cjmg`. Finally, it calls this method on all non-`nil` scope providers, giving each an opportunity to perform arbitrary work before or after invoking `function`.

This method should either invoke `function` once before returning, or throw an error if it’s unable to provide a custom scope.

Issues recorded by this method are associated with `test`.

