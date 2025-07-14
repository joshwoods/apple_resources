

- Swift
- String
-  init(validatingCString:) 

Initializer

# init(validatingCString:)

Creates a new string by copying and validating the null-terminated UTF-8 data referenced by the given pointer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init?(validatingCString nullTerminatedUTF8: UnsafePointer)
```

## Parameters 

`nullTerminatedUTF8`  

A pointer to a null-terminated sequence of UTF-8 code units.

## Discussion

This initializer does not try to repair ill-formed UTF-8 code unit sequences. If any are found, the result of the initializer is `nil`.

The following example calls this initializer with pointers to the contents of two different `CChar` arrays—the first with well-formed UTF-8 code unit sequences and the second with an ill-formed sequence at the end.

```
let validUTF8: [CChar] = [67, 97, 102, -61, -87, 0]
validUTF8.withUnsafeBufferPointer { ptr in
    let s = String(validatingCString: ptr.baseAddress!)
    print(s)
}
// Prints "Optional("Café")"

let invalidUTF8: [CChar] = [67, 97, 102, -61, 0]
invalidUTF8.withUnsafeBufferPointer { ptr in
    let s = String(validatingCString: ptr.baseAddress!)
    print(s)
}
// Prints "nil"
```

## See Also

### Converting a C String

init?&lt;S>(bytes: S, encoding: String.Encoding)

Creates a new string equivalent to the given bytes interpreted in the specified encoding. Note: This API does not interpret embedded nulls as termination of the string. Use `String?(validatingCString:)` instead for null-terminated C strings.

init?(bytesNoCopy: UnsafeMutableRawPointer, length: Int, encoding: String.Encoding, freeWhenDone: Bool)

Creates a new string that contains the specified number of bytes from the given buffer, interpreted in the specified encoding, and optionally frees the buffer.

Deprecated

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

