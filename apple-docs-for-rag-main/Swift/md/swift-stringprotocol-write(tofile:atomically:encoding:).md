

- Swift
- StringProtocol
-  write(toFile:atomically:encoding:) 

Instance Method

# write(toFile:atomically:encoding:)

Writes the contents of the `String` to a file at a given path using a given encoding.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func write(
    toFile path: T,
    atomically useAuxiliaryFile: Bool,
    encoding enc: String.Encoding
) throws where T : StringProtocol
```

