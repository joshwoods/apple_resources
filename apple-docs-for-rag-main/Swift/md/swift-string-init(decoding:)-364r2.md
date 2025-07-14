

- Swift
- String
-  init(decoding:) 

Initializer

# init(decoding:)

On Unix, creates the string `"/"`

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(decoding root: FilePath.Root)
```

## Parameters 

`root`  

The path root to be interpreted as `CInterop.PlatformUnicodeEncoding`.

## Discussion

On Windows, creates a string by interpreting the path root’s content as UTF-16.

If the content of the path root isn’t a well-formed Unicode string, this initializer replaces invalid bytes with U+FFFD. This means that on Windows, conversion to a string and back to a path root might result in a value that’s different from the original path root.

