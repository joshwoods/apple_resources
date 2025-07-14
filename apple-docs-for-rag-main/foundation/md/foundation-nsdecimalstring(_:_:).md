

- Foundation
-  NSDecimalString(\_:\_:) 

Function

# NSDecimalString(\_:\_:)

Returns a string representation of the decimal value appropriate for the specified locale.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func NSDecimalString(
    _ dcm: UnsafePointer,
    _ locale: Any?
) -> String
```

## Parameters 

`dcm`  

The decimal value to represent.

`locale`  

Either an instance of NSLocale or a dictionary with a string value corresponding to the decimalSeparator key.

