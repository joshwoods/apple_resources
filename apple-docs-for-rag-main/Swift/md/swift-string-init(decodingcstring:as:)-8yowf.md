

- Swift
- String
-  init(decodingCString:as:) 

Initializer

# init(decodingCString:as:)

Creates a new string by copying the null-terminated sequence of code units referenced by the given pointer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    decodingCString nullTerminatedCodeUnits: UnsafePointer,
    as encoding: Encoding.Type
) where Encoding : _UnicodeEncoding
```

## Parameters 

`nullTerminatedCodeUnits`  

A pointer to a null-terminated sequence of code units encoded in `encoding`.

`encoding`  

The encoding in which the code units should be interpreted.

## Discussion

If `nullTerminatedCodeUnits` contains ill-formed code unit sequences, this initializer replaces them with the Unicode replacement character (`"\u{FFFD}"`).

