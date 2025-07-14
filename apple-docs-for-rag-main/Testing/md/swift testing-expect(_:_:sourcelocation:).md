

- Swift Testing
-  expect(\_:\_:sourceLocation:) 

Macro

# expect(\_:\_:sourceLocation:)

Check that an expectation has passed after a condition has been evaluated.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
@freestanding(expression)
macro expect(
    _ condition: Bool,
    _ comment: @autoclosure () -> Comment? = nil,
    sourceLocation: SourceLocation = #_sourceLocation
)
```

## Parameters 

`condition`  

The condition to be evaluated.

`comment`  

A comment describing the expectation.

`sourceLocation`  

The source location to which recorded expectations and issues should be attributed.

## Mentioned in 

Testing for errors in Swift code

Migrating a test from XCTest

## Overview

If `condition` evaluates to `false`, an Issue is recorded for the test that is running in the current task.

## See Also

### Checking expectations

macro require(Bool, @autoclosure () -> Comment?, sourceLocation: SourceLocation)

Check that an expectation has passed after a condition has been evaluated and throw an error if it failed.

macro require&lt;T>(T?, @autoclosure () -> Comment?, sourceLocation: SourceLocation) -> T

Unwrap an optional value or, if it is `nil`, fail and throw an error.

