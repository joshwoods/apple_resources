

- System
- FilePath
- FilePath.Root
-  string 

Instance Property

# string

On Unix, this returns `"/"`.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var string: String { get }
```

## Discussion

On Windows, interprets the root’s content as UTF-16 on Windows.

This property is equivalent to calling `String(decoding: root)`.

