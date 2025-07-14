

- Swift
- StringProtocol
-  getCString(\_:maxLength:encoding:) 

Instance Method

# getCString(\_:maxLength:encoding:)

Converts the `String`’s content to a given encoding and stores them in a buffer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func getCString(
    _ buffer: inout [CChar],
    maxLength: Int,
    encoding: String.Encoding
) -> Bool
```

## Discussion

Note

Will store a maximum of `min(buffer.count, maxLength)` bytes.

