

- Foundation
- NSDataDetector
-  init(types:) 

Initializer

# init(types:)

Initializes and returns a data detector instance.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(types checkingTypes: NSTextCheckingTypes) throws
```

## Parameters 

`checkingTypes`  

The checking types. The supported checking types are a subset of the types NSTextCheckingResult.CheckingType. Those constants can be combined using the C-bitwise OR operator.

## Return Value

Returns the newly initialized data detector. If an error was encountered returns `nil`, and `error` contains the error.

## Discussion

Currently, the supported data detectors `checkingTypes` are: date, address, link, `NSTextCheckingTypePhoneNumber`, and `NSTextCheckingTypeTransitInformation`.

Handling Errors in Swift

In Swift, this API is imported as an initializer and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Related Documentation

var checkingTypes: NSTextCheckingTypes

Returns the checking types for the data detector.

