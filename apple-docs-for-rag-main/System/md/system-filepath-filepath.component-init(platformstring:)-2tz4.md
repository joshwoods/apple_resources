

- System
- FilePath
- FilePath.Component
-  init(platformString:) 

Initializer

# init(platformString:)

Creates a file path component by copying bytes from a null-terminated platform string. It is a precondition that a null byte indicates the end of the string. The absence of a null byte will trigger a runtime error.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init?(platformString: [CInterop.PlatformChar])
```

## Parameters 

`platformString`  

A null-terminated platform string.

## Discussion

Returns `nil` if `platformString` is empty, is a root, or has more than one component in it.

- Note It is a precondition that `platformString` must be null-terminated. The absence of a null byte will trigger a runtime error.

