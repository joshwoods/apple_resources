

- System
- FilePath
-  debugDescription 

Instance Property

# debugDescription

A textual representation of the file path, suitable for debugging.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var debugDescription: String { get }
```

## Discussion

If the content of the path isn’t a well-formed Unicode string, this replaces invalid bytes with U+FFFD. See `String.init(decoding:)`

## See Also

### Working with File Paths

var length: Int

The length of the file path, excluding the null terminator.

var description: String

A textual representation of the file path.

