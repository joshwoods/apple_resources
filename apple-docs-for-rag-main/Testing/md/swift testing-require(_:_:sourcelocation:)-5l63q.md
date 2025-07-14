

- Swift Testing
-  require(\_:\_:sourceLocation:) 

Macro

# require(\_:\_:sourceLocation:)

Check that an expectation has passed after a condition has been evaluated and throw an error if it failed.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
@freestanding(expression)
macro require(
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

Migrating a test from XCTest

Testing for errors in Swift code

## Overview

Throws

An instance of ExpectationFailedError if `condition` evaluates to `false`.

If `condition` evaluates to `false`, an Issue is recorded for the test that is running in the current task and an instance of ExpectationFailedError is thrown.

## See Also

### Checking expectations

macro expect(Bool, @autoclosure () -> Comment?, sourceLocation: SourceLocation)

Check that an expectation has passed after a condition has been evaluated.

macro require&lt;T>(T?, @autoclosure () -> Comment?, sourceLocation: SourceLocation) -> T

Unwrap an optional value or, if it is `nil`, fail and throw an error.

