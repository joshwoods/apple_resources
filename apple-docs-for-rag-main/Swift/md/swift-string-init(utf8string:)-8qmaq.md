

- Swift
- String
-  init(utf8String:) 

Initializer

# init(utf8String:)

Creates a string by copying the data from a given null-terminated array of UTF8-encoded bytes.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init?(utf8String bytes: [CChar])
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

init?&lt;Encoding>(validating: some Sequence&lt;Int8>, as: Encoding.Type)

Creates a new string by copying and validating the sequence of code units passed in, according to the specified encoding.

init?(utf8String: UnsafePointer&lt;CChar>)

Creates a string by copying the data from a given null-terminated C array of UTF8-encoded bytes.

init(utf16CodeUnits: UnsafePointer&lt;unichar>, count: Int)

Creates a new string that contains the specified number of characters from the given C array of Unicode characters.

init(utf16CodeUnitsNoCopy: UnsafePointer&lt;unichar>, count: Int, freeWhenDone: Bool)

Creates a new string that contains the specified number of characters from the given C array of UTF-16 code units.

Deprecated

init&lt;C, Encoding>(decoding: C, as: Encoding.Type)

Creates a string from the given Unicode code units in the specified encoding.

