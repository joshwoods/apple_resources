

- Swift
- String
-  init(validatingPlatformString:) 

Initializer

# init(validatingPlatformString:)

Creates a string by interpreting the null-terminated platform string as UTF-8 on Unix and UTF-16 on Windows.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init?(validatingPlatformString platformString: UnsafePointer)
```

## Parameters 

`platformString`  

The null-terminated platform string to be interpreted as `CInterop.PlatformUnicodeEncoding`.

## Discussion

If the contents of the platform string isn’t well-formed Unicode, this initializer returns `nil`.

