

- Swift
- BidirectionalCollection
-  prefixMatch(of:) 

Instance Method

# prefixMatch(of:)

Matches part of the regex, starting at the beginning, where the regex is created by the given closure.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func prefixMatch(@RegexComponentBuilder of content: () -> some RegexComponent) -> Regex.Match?
```

Available when `SubSequence` is `Substring`.

## Parameters 

`content`  

A closure that returns a regex to match against.

## Return Value

The match if there is one, or `nil` if none.

