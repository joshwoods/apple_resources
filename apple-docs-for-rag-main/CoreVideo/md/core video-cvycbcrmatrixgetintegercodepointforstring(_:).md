

- Core Video
-  CVYCbCrMatrixGetIntegerCodePointForString(\_:) 

Function

# CVYCbCrMatrixGetIntegerCodePointForString(\_:)

Returns the standard integer code point corresponding to the Core Video YCbCr matrix string that you specify.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func CVYCbCrMatrixGetIntegerCodePointForString(_ yCbCrMatrixString: CFString?) -> Int32
```

## Parameters 

`yCbCrMatrixString`  

A Core Video YCbCr matrix string. See Image Buffer YCbCr Matrix Constants for possible values.

## Return Value

The code point corresponding to the YCbCr matrix string, or `2` (unknown) if the string is nil or the system doesn’t recognize it.

## See Also

### Converting between strings and integer code points

func CVColorPrimariesGetIntegerCodePointForString(CFString?) -> Int32

Returns the standard integer code point corresponding to the Core Video color primaries constant string that you specify.

func CVColorPrimariesGetStringForIntegerCodePoint(Int32) -> Unmanaged&lt;CFString>?

Returns the Core Video color primaries string corresponding to the standard integer code point that you specify.

func CVTransferFunctionGetIntegerCodePointForString(CFString?) -> Int32

Returns the standard integer code point corresponding to the Core Video transfer function string that you specify.

func CVTransferFunctionGetStringForIntegerCodePoint(Int32) -> Unmanaged&lt;CFString>?

Returns the Core Video transfer function string corresponding to the standard integer code point that you specify.

func CVYCbCrMatrixGetStringForIntegerCodePoint(Int32) -> Unmanaged&lt;CFString>?

Returns the Core Video YCbCr matrix string corresponding to the standard integer code point that you specify.

