

- Core Video
-  CVTransferFunctionGetIntegerCodePointForString(\_:) 

Function

# CVTransferFunctionGetIntegerCodePointForString(\_:)

Returns the standard integer code point corresponding to the Core Video transfer function string that you specify.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func CVTransferFunctionGetIntegerCodePointForString(_ transferFunctionString: CFString?) -> Int32
```

## Parameters 

`transferFunctionString`  

A Core Video transfer function string. See Image Buffer Transfer Function Constants for possible values.

## Return Value

The code point corresponding to the transfer function string, or `2` (unknown) if the string is nil or the system doesn’t recognize it.

## See Also

### Converting between strings and integer code points

func CVColorPrimariesGetIntegerCodePointForString(CFString?) -> Int32

Returns the standard integer code point corresponding to the Core Video color primaries constant string that you specify.

func CVColorPrimariesGetStringForIntegerCodePoint(Int32) -> Unmanaged&lt;CFString>?

Returns the Core Video color primaries string corresponding to the standard integer code point that you specify.

func CVTransferFunctionGetStringForIntegerCodePoint(Int32) -> Unmanaged&lt;CFString>?

Returns the Core Video transfer function string corresponding to the standard integer code point that you specify.

func CVYCbCrMatrixGetIntegerCodePointForString(CFString?) -> Int32

Returns the standard integer code point corresponding to the Core Video YCbCr matrix string that you specify.

func CVYCbCrMatrixGetStringForIntegerCodePoint(Int32) -> Unmanaged&lt;CFString>?

Returns the Core Video YCbCr matrix string corresponding to the standard integer code point that you specify.

