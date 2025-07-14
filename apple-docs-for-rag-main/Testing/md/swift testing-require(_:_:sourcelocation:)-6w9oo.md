

- Swift Testing
-  require(\_:\_:sourceLocation:) 

Macro

# require(\_:\_:sourceLocation:)

Unwrap an optional value or, if it is `nil`, fail and throw an error.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
@freestanding(expression)
macro require(
    _ optionalValue: T?,
    _ comment: @autoclosure () -> Comment? = nil,
    sourceLocation: SourceLocation = #_sourceLocation
) -> T
```

## Parameters 

`optionalValue`  

The optional value to be unwrapped.

`comment`  

A comment describing the expectation.

`sourceLocation`  

The source location to which recorded expectations and issues should be attributed.

## Return Value

The unwrapped value of `optionalValue`.

## Mentioned in 

Migrating a test from XCTest

## Overview

Throws

An instance of ExpectationFailedError if `optionalValue` is `nil`.

If `optionalValue` is `nil`, an Issue is recorded for the test that is running in the current task and an instance of ExpectationFailedError is thrown.

## See Also

### Checking expectations

macro expect(Bool, @autoclosure () -> Comment?, sourceLocation: SourceLocation)

Check that an expectation has passed after a condition has been evaluated.

macro require(Bool, @autoclosure () -> Comment?, sourceLocation: SourceLocation)

Check that an expectation has passed after a condition has been evaluated and throw an error if it failed.

