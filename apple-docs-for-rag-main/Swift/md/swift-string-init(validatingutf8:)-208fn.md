

- Swift
- String
-  init(validatingUTF8:) 

Initializer

# init(validatingUTF8:)

Creates a new string by copying and validating the null-terminated UTF-8 data referenced by the given pointer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+SwiftDeprecated

``` source
init?(validatingUTF8 cString: UnsafePointer)
```

## Parameters 

`cString`  

A pointer to a null-terminated sequence of UTF-8 code units.

## Discussion

This initializer does not try to repair ill-formed UTF-8 code unit sequences. If any are found, the result of the initializer is `nil`.

The following example calls this initializer with pointers to the contents of two different `CChar` arrays—the first with well-formed UTF-8 code unit sequences and the second with an ill-formed sequence at the end.

```
let validUTF8: [CChar] = [67, 97, 102, -61, -87, 0]
validUTF8.withUnsafeBufferPointer { ptr in
    let s = String(validatingUTF8: ptr.baseAddress!)
    print(s)
}
// Prints "Optional("Café")"

let invalidUTF8: [CChar] = [67, 97, 102, -61, 0]
invalidUTF8.withUnsafeBufferPointer { ptr in
    let s = String(validatingUTF8: ptr.baseAddress!)
    print(s)
}
// Prints "nil"
```

Note

This initializer has been renamed. Use `String.init?(validatingCString:)` instead.

## See Also

### Creating a String from Unicode Data

init(Unicode.Scalar)

init?(data: Data, encoding: String.Encoding)

Returns a `String` initialized by converting given `data` into Unicode characters using a given `encoding`.

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

init(utf16CodeUnitsNoCopy: UnsafePointer&lt;unichar>, count: Int, freeWhenDone: Bool)

Creates a new string that contains the specified number of characters from the given C array of UTF-16 code units.

Deprecated

init&lt;C, Encoding>(decoding: C, as: Encoding.Type)

Creates a string from the given Unicode code units in the specified encoding.

