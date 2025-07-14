

- Swift
- BidirectionalCollection
-  wholeMatch(of:) 

Instance Method

# wholeMatch(of:)

Matches a regex in its entirety, where the regex is created by the given closure.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func wholeMatch(@RegexComponentBuilder of content: () -> some RegexComponent) -> Regex.Match?
```

Available when `SubSequence` is `Substring`.

## Parameters 

`content`  

A closure that returns a regex to match against.

## Return Value

The match if there is one, or `nil` if none.

