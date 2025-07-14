

- Swift
- StringProtocol
-  write(to:atomically:encoding:) 

Instance Method

# write(to:atomically:encoding:)

Writes the contents of the `String` to the URL specified by url using the specified encoding.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func write(
    to url: URL,
    atomically useAuxiliaryFile: Bool,
    encoding enc: String.Encoding
) throws
```

