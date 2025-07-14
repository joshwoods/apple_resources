

- Swift
- StringProtocol
-  getLineStart(\_:end:contentsEnd:for:) 

Instance Method

# getLineStart(\_:end:contentsEnd:for:)

Returns by reference the beginning of the first line and the end of the last line touched by the given range.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func getLineStart(
    _ start: UnsafeMutablePointer,
    end: UnsafeMutablePointer,
    contentsEnd: UnsafeMutablePointer,
    for range: some RangeExpression
)
```

