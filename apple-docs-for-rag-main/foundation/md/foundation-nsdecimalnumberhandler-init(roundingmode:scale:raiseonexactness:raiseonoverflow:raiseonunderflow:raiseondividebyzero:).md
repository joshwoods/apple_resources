

- Foundation
- NSDecimalNumberHandler
-  init(roundingMode:scale:raiseOnExactness:raiseOnOverflow:raiseOnUnderflow:raiseOnDivideByZero:) 

Initializer

# init(roundingMode:scale:raiseOnExactness:raiseOnOverflow:raiseOnUnderflow:raiseOnDivideByZero:)

Returns an `NSDecimalNumberHandler` object initialized so it behaves as specified by the method’s arguments.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    roundingMode: NSDecimalNumber.RoundingMode,
    scale: Int16,
    raiseOnExactness exact: Bool,
    raiseOnOverflow overflow: Bool,
    raiseOnUnderflow underflow: Bool,
    raiseOnDivideByZero divideByZero: Bool
)
```

## Parameters 

`roundingMode`  

The rounding mode to use. There are four possible values: `NSRoundUp`, `NSRoundDown`, `NSRoundPlain`, and `NSRoundBankers`.

`scale`  

The number of digits a rounded value should have after its decimal point.

`exact`  

If true, in the event of an exactness error the handler will raise an exception, otherwise it will ignore the error and return control to the calling method.

`overflow`  

If true, in the event of an overflow error the handler will raise an exception, otherwise it will ignore the error and return control to the calling method

`underflow`  

If true, in the event of an underflow error the handler will raise an exception, otherwise it will ignore the error and return control to the calling method

`divideByZero`  

If true, in the event of a divide by zero error the handler will raise an exception, otherwise it will ignore the error and return control to the calling method

## Return Value

An initialized `NSDecimalNumberHandler` object initialized with customized behavior. The returned object might be different than the original receiver.

## Discussion

See the NSDecimalNumberBehaviors protocol specification for a complete explanation of the possible behaviors.

