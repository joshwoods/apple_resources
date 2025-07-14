

- Core Video
-  Core Video Functions 

API Collection

# Core Video Functions

## Topics

### Converting between strings and integer code points

func CVColorPrimariesGetIntegerCodePointForString(CFString?) -> Int32

Returns the standard integer code point corresponding to the Core Video color primaries constant string that you specify.

func CVColorPrimariesGetStringForIntegerCodePoint(Int32) -> Unmanaged&lt;CFString>?

Returns the Core Video color primaries string corresponding to the standard integer code point that you specify.

func CVTransferFunctionGetIntegerCodePointForString(CFString?) -> Int32

Returns the standard integer code point corresponding to the Core Video transfer function string that you specify.

func CVTransferFunctionGetStringForIntegerCodePoint(Int32) -> Unmanaged&lt;CFString>?

Returns the Core Video transfer function string corresponding to the standard integer code point that you specify.

func CVYCbCrMatrixGetIntegerCodePointForString(CFString?) -> Int32

Returns the standard integer code point corresponding to the Core Video YCbCr matrix string that you specify.

func CVYCbCrMatrixGetStringForIntegerCodePoint(Int32) -> Unmanaged&lt;CFString>?

Returns the Core Video YCbCr matrix string corresponding to the standard integer code point that you specify.

### Functions

func CVIsCompressedPixelFormatAvailable(OSType) -> Bool

func CVPixelBufferCopyCreationAttributes(CVPixelBuffer) -> CFDictionary

## See Also

### Reference

Core Video Enumerations

Core Video Constants

