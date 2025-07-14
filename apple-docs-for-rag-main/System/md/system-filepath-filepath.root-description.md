

- System
- FilePath
- FilePath.Root
-  description 

Instance Property

# description

A textual representation of the path root.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var description: String { get }
```

## Discussion

If the content of the path root isn’t a well-formed Unicode string, this replaces invalid bytes with U+FFFD. See `String.init(decoding:)`.

