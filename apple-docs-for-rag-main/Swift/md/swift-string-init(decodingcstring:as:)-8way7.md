

- Swift
- String
-  init(decodingCString:as:) 

Initializer

# init(decodingCString:as:)

Creates a new string by copying the null-terminated sequence of code units referenced by the given array.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+SwiftDeprecated

``` source
init(
    decodingCString nullTerminatedCodeUnits: [Encoding.CodeUnit],
    as encoding: Encoding.Type
) where Encoding : _UnicodeEncoding
```

## Parameters 

`nullTerminatedCodeUnits`  

An array containing a null-terminated sequence of code units encoded in `encoding`.

`encoding`  

The encoding in which the code units should be interpreted.

## Discussion

If `nullTerminatedCodeUnits` contains ill-formed code unit sequences, this initializer replaces them with the Unicode replacement character (`"\u{FFFD}"`).

Note

This initializer is deprecated. Use the initializer `String.init(decoding: array, as: Encoding.self)` instead, remembering that “\0” is a valid character in Swift.

## See Also

### Converting a C String

init?&lt;S>(bytes: S, encoding: String.Encoding)

Creates a new string equivalent to the given bytes interpreted in the specified encoding. Note: This API does not interpret embedded nulls as termination of the string. Use `String?(validatingCString:)` instead for null-terminated C strings.

init?(bytesNoCopy: UnsafeMutableRawPointer, length: Int, encoding: String.Encoding, freeWhenDone: Bool)

Creates a new string that contains the specified number of bytes from the given buffer, interpreted in the specified encoding, and optionally frees the buffer.

Deprecated

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

static func decodeCString&lt;Encoding>(UnsafePointer&lt;Encoding.CodeUnit>?, as: Encoding.Type, repairingInvalidCodeUnits: Bool) -> (result: String, repairsMade: Bool)?

Creates a new string by copying the null-terminated data referenced by the given pointer using the specified encoding.

