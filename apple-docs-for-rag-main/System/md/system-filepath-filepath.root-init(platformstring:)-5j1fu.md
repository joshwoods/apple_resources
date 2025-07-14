

- System
- FilePath
- FilePath.Root
-  init(platformString:) 

Initializer

# init(platformString:)

Creates a file path root by copying bytes from a null-terminated platform string.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init?(platformString: UnsafePointer)
```

## Parameters 

`platformString`  

A pointer to a null-terminated platform string.

## Discussion

Returns `nil` if `platformString` is empty or is not a root.

