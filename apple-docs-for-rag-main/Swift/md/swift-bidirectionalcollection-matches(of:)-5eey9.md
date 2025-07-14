

- Swift
- BidirectionalCollection
-  matches(of:) 

Instance Method

# matches(of:)

Returns a collection containing all non-overlapping matches of the regex, created by the given closure.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func matches(@RegexComponentBuilder of content: () -> some RegexComponent) -> [Regex.Match]
```

Available when `SubSequence` is `Substring`.

## Parameters 

`content`  

A closure that returns the regex to search for.

## Return Value

A collection of matches for the regex returned by `content`. If no matches are found, the returned collection is empty.

