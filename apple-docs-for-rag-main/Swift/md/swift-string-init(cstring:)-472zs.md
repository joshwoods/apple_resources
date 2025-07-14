

- Swift
- String
-  init(cString:) 

Initializer

# init(cString:)

Creates a new string by copying the null-terminated UTF-8 data referenced by the given array.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+SwiftDeprecated

``` source
init(cString nullTerminatedUTF8: [UInt8])
```

## Parameters 

`nullTerminatedUTF8`  

An array containing a null-terminated UTF-8 code unit sequence.

## Discussion

This is identical to `init(cString: [CChar])` but operates on an unsigned sequence of bytes.

Note

This initializer is deprecated. Use the initializer `String.init(decoding: array, as: UTF8.self)` instead, remembering that “\0” is a valid character in Swift.

