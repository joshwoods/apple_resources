

- Swift
- Substring
-  init(decodingCString:as:) 

Initializer

# init(decodingCString:as:)

Creates a string from the null-terminated sequence of bytes at the given pointer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    decodingCString nullTerminatedCodeUnits: UnsafePointer,
    as sourceEncoding: Encoding.Type
) where Encoding : _UnicodeEncoding
```

## Parameters 

`nullTerminatedCodeUnits`  

A pointer to a sequence of contiguous code units in the encoding specified in `sourceEncoding`, ending just before the first zero code unit.

`sourceEncoding`  

The encoding in which the code units should be interpreted.

