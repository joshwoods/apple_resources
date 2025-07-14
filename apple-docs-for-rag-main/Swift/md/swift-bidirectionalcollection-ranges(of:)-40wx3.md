

- Swift
- BidirectionalCollection
-  ranges(of:) 

Instance Method

# ranges(of:)

Finds and returns the ranges of the all occurrences of a given sequence within the collection.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func ranges(of regex: some RegexComponent) -> [Range]
```

Available when `SubSequence` is `Substring`.

## Parameters 

`regex`  

The regex to search for.

## Return Value

A collection or ranges in the receiver of all occurrences of `regex`. Returns an empty collection if `regex` is not found.

