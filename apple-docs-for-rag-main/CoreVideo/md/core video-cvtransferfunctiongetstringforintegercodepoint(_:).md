

- Core Video
-  CVTransferFunctionGetStringForIntegerCodePoint(\_:) 

Function

# CVTransferFunctionGetStringForIntegerCodePoint(\_:)

Returns the Core Video transfer function string corresponding to the standard integer code point that you specify.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func CVTransferFunctionGetStringForIntegerCodePoint(_ transferFunctionCodePoint: Int32) -> Unmanaged?
```

## Parameters 

`transferFunctionCodePoint`  

The standard integer code point.

## Return Value

The transfer function string corresponding to the code point (See Image Buffer Transfer Function Constants for possible values.), or nil if the code point is `2` (unknown) or the system doesn’t recognize it.

## See Also

### Converting between strings and integer code points

func CVColorPrimariesGetIntegerCodePointForString(CFString?) -> Int32

Returns the standard integer code point corresponding to the Core Video color primaries constant string that you specify.

func CVColorPrimariesGetStringForIntegerCodePoint(Int32) -> Unmanaged&lt;CFString>?

Returns the Core Video color primaries string corresponding to the standard integer code point that you specify.

func CVTransferFunctionGetIntegerCodePointForString(CFString?) -> Int32

Returns the standard integer code point corresponding to the Core Video transfer function string that you specify.

func CVYCbCrMatrixGetIntegerCodePointForString(CFString?) -> Int32

Returns the standard integer code point corresponding to the Core Video YCbCr matrix string that you specify.

func CVYCbCrMatrixGetStringForIntegerCodePoint(Int32) -> Unmanaged&lt;CFString>?

Returns the Core Video YCbCr matrix string corresponding to the standard integer code point that you specify.

