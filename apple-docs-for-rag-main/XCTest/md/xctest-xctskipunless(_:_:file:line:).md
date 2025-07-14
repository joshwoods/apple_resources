

- XCTest
-  XCTSkipUnless(\_:\_:file:line:) 

Function

# XCTSkipUnless(\_:\_:file:line:)

Skips remaining tests in a test method unless the specified condition is met.

``` source
func XCTSkipUnless(
    _ expression: @autoclosure () throws -> Bool,
    _ message: @autoclosure () -> String? = nil,
    file: StaticString = #filePath,
    line: UInt = #line
) throws
```

## Parameters 

`expression`  

A Boolean expression.

`message`  

An optional description of the skip.

`file`  

The file where the skip occurs. The default is the filename of the test case where you call this function.

`line`  

The line number where the skip occurs. The default is the line number where you call this function.

## Discussion

Call this method to skip any remaining code and assertions in the test method when `expression` evaluates to `false`, and mark the test method as skipped. If a test failure occurs in the test method before the skip, the test runner marks the test method as failed.

## See Also

### Methods for Skipping Tests

func XCTSkipIf(@autoclosure () throws -> Bool, @autoclosure () -> String?, file: StaticString, line: UInt) throws

Skips remaining tests in a test method if the specified condition is met.

struct XCTSkip

An error that causes the current test to cease executing and the test runner to mark the test as skipped when the test throws the error.

