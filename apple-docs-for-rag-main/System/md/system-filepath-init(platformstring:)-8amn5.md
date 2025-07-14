

- System
- FilePath
-  init(platformString:) 

Initializer

# init(platformString:)

Creates a file path by copying bytes from a null-terminated platform string.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(platformString: [CInterop.PlatformChar])
```

## Parameters 

`platformString`  

A null-terminated platform string.

## Discussion

- Note It is a precondition that `platformString` must be null-terminated. The absence of a null byte will trigger a runtime error.

