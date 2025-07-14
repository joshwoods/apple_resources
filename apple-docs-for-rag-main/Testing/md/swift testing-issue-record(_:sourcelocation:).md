

- Swift Testing
- Issue
-  record(\_:sourceLocation:) 

Type Method

# record(\_:sourceLocation:)

Record an issue when a running test fails unexpectedly.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
@discardableResult
static func record(
    _ comment: Comment? = nil,
    sourceLocation: SourceLocation = #_sourceLocation
) -> Issue
```

## Parameters 

`comment`  

A comment describing the expectation.

`sourceLocation`  

The source location to which the issue should be attributed.

## Return Value

The issue that was recorded.

## Mentioned in 

Migrating a test from XCTest

## Discussion

Use this function if, while running a test, an issue occurs that cannot be represented as an expectation (using the expect(_:_:sourceLocation:) or require(_:_:sourceLocation:) macros.)

