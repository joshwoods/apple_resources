

- Swift
- StringProtocol
-  appendingFormat(\_:\_:) 

Instance Method

# appendingFormat(\_:\_:)

Returns a string created by appending a string constructed from a given format string and the following arguments.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func appendingFormat(
    _ format: T,
    _ arguments: any CVarArg...
) -> String where T : StringProtocol
```

