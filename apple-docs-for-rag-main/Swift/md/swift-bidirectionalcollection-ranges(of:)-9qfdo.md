

- Swift
- BidirectionalCollection
-  ranges(of:) 

Instance Method

# ranges(of:)

Returns the ranges of the all non-overlapping matches for the regex within this collection, where the regex is created by the given closure.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func ranges(@RegexComponentBuilder of content: () -> some RegexComponent) -> [Range]
```

Available when `SubSequence` is `Substring`.

## Parameters 

`content`  

A closure that returns a regex to search for.

## Return Value

A collection of ranges of all matches for the regex returned by `content`. Returns an empty collection if no match for the regex is found.

