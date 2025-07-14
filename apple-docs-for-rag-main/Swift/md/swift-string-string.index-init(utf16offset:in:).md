

- Swift
- String
- String.Index
-  init(utf16Offset:in:) 

Initializer

# init(utf16Offset:in:)

Creates a new index at the specified UTF-16 code unit offset

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    utf16Offset offset: Int,
    in s: S
) where S : StringProtocol
```

## Parameters 

`offset`  

An offset in UTF-16 code units.

