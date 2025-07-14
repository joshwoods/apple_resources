

- Swift
- String
-  decodeCString(\_:as:repairingInvalidCodeUnits:) 

Type Method

# decodeCString(\_:as:repairingInvalidCodeUnits:)

Creates a new string by copying the null-terminated data referenced by the given pointer using the specified encoding.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func decodeCString(
    _ cString: UnsafePointer?,
    as encoding: Encoding.Type,
    repairingInvalidCodeUnits isRepairing: Bool = true
) -> (result: String, repairsMade: Bool)? where Encoding : _UnicodeEncoding
```

## Parameters 

`cString`  

A pointer to a null-terminated sequence of code units encoded in `encoding`.

`encoding`  

The Unicode encoding of the data referenced by `cString`.

`isRepairing`  

Pass `true` to create a new string, even when the data referenced by `cString` contains ill-formed sequences. Ill-formed sequences are replaced with the Unicode replacement character (`"\u{FFFD}"`). Pass `false` to interrupt the creation of the new string if an ill-formed sequence is detected.

## Return Value

A tuple with the new string and a Boolean value that indicates whether any repairs were made. If `isRepairing` is `false` and an ill-formed sequence is detected, this method returns `nil`.

## Discussion

When you pass `true` as `isRepairing`, this method replaces ill-formed sequences with the Unicode replacement character (`"\u{FFFD}"`); otherwise, an ill-formed sequence causes this method to stop decoding and return `nil`.

The following example calls this method with pointers to the contents of two different `CChar` arrays—the first with well-formed UTF-8 code unit sequences and the second with an ill-formed sequence at the end.

```
let validUTF8: [UInt8] = [67, 97, 102, 195, 169, 0]
validUTF8.withUnsafeBufferPointer { ptr in
    let s = String.decodeCString(ptr.baseAddress,
                                 as: UTF8.self,
                                 repairingInvalidCodeUnits: true)
    print(s)
}
// Prints "Optional((result: "Café", repairsMade: false))"

let invalidUTF8: [UInt8] = [67, 97, 102, 195, 0]
invalidUTF8.withUnsafeBufferPointer { ptr in
    let s = String.decodeCString(ptr.baseAddress,
                                 as: UTF8.self,
                                 repairingInvalidCodeUnits: true)
    print(s)
}
// Prints "Optional((result: "Caf�", repairsMade: true))"
```

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

init&lt;Encoding>(decodingCString: [Encoding.CodeUnit], as: Encoding.Type)

Creates a new string by copying the null-terminated sequence of code units referenced by the given array.

