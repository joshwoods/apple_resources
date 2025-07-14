

- System
- FilePath
- FilePath.Root
-  debugDescription 

Instance Property

# debugDescription

A textual representation of the path root, suitable for debugging.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var debugDescription: String { get }
```

## Discussion

If the content of the path root isn’t a well-formed Unicode string, this replaces invalid bytes with U+FFFD. See `String.init(decoding:)`.

