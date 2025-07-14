

- Swift
- StringProtocol
-  init(decoding:as:) 

Initializer

# init(decoding:as:)

Creates a string from the given Unicode code units in the specified encoding.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    decoding codeUnits: C,
    as sourceEncoding: Encoding.Type
) where C : Collection, Encoding : _UnicodeEncoding, C.Element == Encoding.CodeUnit
```

**Required**

## Parameters 

`codeUnits`  

A collection of code units encoded in the encoding specified in `sourceEncoding`.

`sourceEncoding`  

The encoding in which `codeUnits` should be interpreted.

