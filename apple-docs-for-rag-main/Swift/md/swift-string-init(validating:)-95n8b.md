

- Swift
- String
-  init(validating:) 

Initializer

# init(validating:)

Creates a string from a path component, validating its contents as UTF-8 on Unix and UTF-16 on Windows.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init?(validating component: FilePath.Component)
```

## Parameters 

`component`  

The path component to be interpreted as `CInterop.PlatformUnicodeEncoding`.

## Discussion

If the contents of the path component isn’t a well-formed Unicode string, this initializer returns `nil`.

