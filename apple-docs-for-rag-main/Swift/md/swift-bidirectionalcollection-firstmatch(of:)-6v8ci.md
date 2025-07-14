

- Swift
- BidirectionalCollection
-  firstMatch(of:) 

Instance Method

# firstMatch(of:)

Returns the first match for the regex within this collection, where the regex is created by the given closure.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func firstMatch(@RegexComponentBuilder of content: () -> some RegexComponent) -> Regex.Match?
```

Available when `SubSequence` is `Substring`.

## Parameters 

`content`  

A closure that returns the regex to search for.

## Return Value

The first match for the regex created by `content` in this collection, or `nil` if no match is found.

