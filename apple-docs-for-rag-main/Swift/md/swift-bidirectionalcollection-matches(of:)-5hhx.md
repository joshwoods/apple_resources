

- Swift
- BidirectionalCollection
-  matches(of:) 

Instance Method

# matches(of:)

Returns a collection containing all matches of the specified regex.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func matches(of r: some RegexComponent) -> [Regex.Match]
```

Available when `SubSequence` is `Substring`.

## Return Value

A collection of matches of `regex`.

