

- Swift
- String
-  init(validating:as:) 

Initializer

# init(validating:as:)

Creates a new string by copying and validating the sequence of code units passed in, according to the specified encoding.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
init?(
    validating codeUnits: some Sequence,
    as encoding: Encoding.Type
) where Encoding : _UnicodeEncoding, Encoding.CodeUnit == UInt8
```

## Parameters 

`codeUnits`  

A sequence of code units that encode a `String`

`encoding`  

A conformer to `Unicode.Encoding` that can decode `codeUnits` as `UInt8`

## Discussion

This initializer does not try to repair ill-formed code unit sequences. If any are found, the result of the initializer is `nil`.

The following example calls this initializer with the contents of two different arrays—first with a well-formed UTF-8 code unit sequence and then with an ill-formed ASCII code unit sequence.

```
let validUTF8: [Int8] = [67, 97, 0, 102, -61, -87]
let valid = String(validating: validUTF8, as: UTF8.self)
print(valid ?? "nil")
// Prints "Café"

let invalidASCII: [Int8] = [67, 97, -5]
let invalid = String(validating: invalidASCII, as: Unicode.ASCII.self)
print(invalid ?? "nil")
// Prints "nil"
```

## See Also

### Creating a String from Unicode Data

init(Unicode.Scalar)

init?(data: Data, encoding: String.Encoding)

Returns a `String` initialized by converting given `data` into Unicode characters using a given `encoding`.

init?(validatingUTF8: UnsafePointer&lt;CChar>)

Creates a new string by copying and validating the null-terminated UTF-8 data referenced by the given pointer.

init?&lt;Encoding>(validating: some Sequence, as: Encoding.Type)

Creates a new string by copying and validating the sequence of code units passed in, according to the specified encoding.

init?(utf8String: [CChar])

Creates a string by copying the data from a given null-terminated array of UTF8-encoded bytes.

init?(utf8String: UnsafePointer&lt;CChar>)

Creates a string by copying the data from a given null-terminated C array of UTF8-encoded bytes.

init(utf16CodeUnits: UnsafePointer&lt;unichar>, count: Int)

Creates a new string that contains the specified number of characters from the given C array of Unicode characters.

init(utf16CodeUnitsNoCopy: UnsafePointer&lt;unichar>, count: Int, freeWhenDone: Bool)

Creates a new string that contains the specified number of characters from the given C array of UTF-16 code units.

Deprecated

init&lt;C, Encoding>(decoding: C, as: Encoding.Type)

Creates a string from the given Unicode code units in the specified encoding.

