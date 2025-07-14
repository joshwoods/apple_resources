

- XCTest
-  XCTFail(\_:file:line:) 

Function

# XCTFail(\_:file:line:)

This function generates a failure immediately and unconditionally.

``` source
func XCTFail(
    _ message: String = "",
    file: StaticString = #filePath,
    line: UInt = #line
)
```

## Parameters 

`message`  

An optional description of the assertion, for inclusion in test results.

`file`  

The file where the failure occurs. The default is the filename of the test case where you call this function.

`line`  

The line number where the failure occurs. The default is the line number where you call this function.

