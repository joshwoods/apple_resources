

- Swift Testing
- Issue
-  record(\_:\_:sourceLocation:) 

Type Method

# record(\_:\_:sourceLocation:)

Record a new issue when a running test unexpectedly catches an error.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
@discardableResult
static func record(
    _ error: any Error,
    _ comment: Comment? = nil,
    sourceLocation: SourceLocation = #_sourceLocation
) -> Issue
```

## Parameters 

`error`  

The error that caused the issue.

`comment`  

A comment describing the expectation.

`sourceLocation`  

The source location to which the issue should be attributed.

## Return Value

The issue that was recorded.

## Discussion

This function can be used if an unexpected error is caught while running a test and it should be treated as a test failure. If an error is thrown from a test function, it is automatically recorded as an issue and this function does not need to be used.

