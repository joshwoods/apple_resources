

- Swift
- String
-  init(utf16CodeUnitsNoCopy:count:freeWhenDone:) Deprecated

Initializer

# init(utf16CodeUnitsNoCopy:count:freeWhenDone:)

Creates a new string that contains the specified number of characters from the given C array of UTF-16 code units.

iOS 8.0–16.0DeprecatediPadOS 8.0–16.0DeprecatedMac Catalyst 8.0–16.0DeprecatedmacOS 10.10–13.0DeprecatedtvOS 9.0–16.0DeprecatedvisionOS 1.0+watchOS 2.0–9.0Deprecated

``` source
init(
    utf16CodeUnitsNoCopy: UnsafePointer,
    count: Int,
    freeWhenDone flag: Bool
)
```

Deprecated

String does not support no-copy initialization

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

init?(utf8String: [CChar])

Creates a string by copying the data from a given null-terminated array of UTF8-encoded bytes.

init?(utf8String: UnsafePointer&lt;CChar>)

Creates a string by copying the data from a given null-terminated C array of UTF8-encoded bytes.

init(utf16CodeUnits: UnsafePointer&lt;unichar>, count: Int)

Creates a new string that contains the specified number of characters from the given C array of Unicode characters.

init&lt;C, Encoding>(decoding: C, as: Encoding.Type)

Creates a string from the given Unicode code units in the specified encoding.

