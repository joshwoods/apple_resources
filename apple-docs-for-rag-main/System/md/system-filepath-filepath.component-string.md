

- System
- FilePath
- FilePath.Component
-  string 

Instance Property

# string

Creates a string by interpreting the component’s content as UTF-8 on Unix and UTF-16 on Windows.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var string: String { get }
```

## Discussion

This property is equivalent to calling `String(decoding: component)`.

