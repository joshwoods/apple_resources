

- Swift
- String
-  init(bytesNoCopy:length:encoding:freeWhenDone:) Deprecated

Initializer

# init(bytesNoCopy:length:encoding:freeWhenDone:)

Creates a new string that contains the specified number of bytes from the given buffer, interpreted in the specified encoding, and optionally frees the buffer.

iOS 8.0–16.0DeprecatediPadOS 8.0–16.0DeprecatedMac Catalyst 8.0–16.0DeprecatedmacOS 10.10–13.0DeprecatedtvOS 9.0–16.0DeprecatedvisionOS 1.0+watchOS 2.0–9.0Deprecated

``` source
init?(
    bytesNoCopy bytes: UnsafeMutableRawPointer,
    length: Int,
    encoding: String.Encoding,
    freeWhenDone flag: Bool
)
```

Deprecated

String does not support no-copy initialization

## Discussion

Warning

This initializer is not memory-safe!

## See Also

### Converting a C String

init?&lt;S>(bytes: S, encoding: String.Encoding)

Creates a new string equivalent to the given bytes interpreted in the specified encoding. Note: This API does not interpret embedded nulls as termination of the string. Use `String?(validatingCString:)` instead for null-terminated C strings.

init?(validatingCString: UnsafePointer&lt;CChar>)

Creates a new string by copying and validating the null-terminated UTF-8 data referenced by the given pointer.

init?(validatingCString: [CChar])

Creates a new string by copying and validating the null-terminated UTF-8 data referenced by the given array.

init(cString: UnsafePointer&lt;CChar>)

Creates a new string by copying the null-terminated UTF-8 data referenced by the given pointer.

init(cString: UnsafePointer&lt;UInt8>)

Creates a new string by copying the null-terminated UTF-8 data referenced by the given pointer.

init?(cString: [CChar], encoding: String.Encoding)

Produces a string by copying the null-terminated bytes in a given array, interpreted according to a given encoding.

init?(cString: UnsafePointer&lt;CChar>, encoding: String.Encoding)

Produces a string by copying the null-terminated bytes in a given C array, interpreted according to a given encoding.

init&lt;Encoding>(decodingCString: [Encoding.CodeUnit], as: Encoding.Type)

Creates a new string by copying the null-terminated sequence of code units referenced by the given array.

static func decodeCString&lt;Encoding>(UnsafePointer&lt;Encoding.CodeUnit>?, as: Encoding.Type, repairingInvalidCodeUnits: Bool) -> (result: String, repairsMade: Bool)?

Creates a new string by copying the null-terminated data referenced by the given pointer using the specified encoding.

