

- Swift Testing
- TestScoping
-  provideScope(for:testCase:performing:) 

Instance Method

# provideScope(for:testCase:performing:)

Provide custom execution scope for a function call which is related to the specified test and/or test case.

Swift 6.1+Xcode 16.3+

``` source
func provideScope(
    for test: Test,
    testCase: Test.Case?,
    performing function: () async throws -> Void
) async throws
```

**Required**

## Parameters 

`test`  

The test under which `function` is being performed.

`testCase`  

The test case, if any, under which `function` is being performed. When invoked on a suite, the value of this argument is `nil`.

`function`  

The function to perform. If `test` represents a test suite, this function encapsulates running all the tests in that suite. If `test` represents a test function, this function is the body of that test function (including all cases if it is parameterized.)

## Discussion

Throws

Whatever is thrown by `function`, or an error preventing this type from providing a custom scope correctly. An error thrown from this method is recorded as an issue associated with `test`. If an error is thrown before `function` is called, the corresponding test will not run.

When the testing library is preparing to run a test, it starts by finding all traits applied to that test, including those inherited from containing suites. It begins with inherited suite traits, sorting them outermost-to-innermost, and if the test is a function, it then adds all traits applied directly to that functions in the order they were applied (left-to-right). It then asks each trait for its scope provider (if any) by calling scopeProvider(for:testCase:). Finally, it calls this method on all non-`nil` scope providers, giving each an opportunity to perform arbitrary work before or after invoking `function`.

This method should either invoke `function` once before returning or throw an error if it is unable to provide a custom scope.

Issues recorded by this method are associated with `test`.

