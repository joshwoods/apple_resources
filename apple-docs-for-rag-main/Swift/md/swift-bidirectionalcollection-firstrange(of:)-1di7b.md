

- Swift
- BidirectionalCollection
-  firstRange(of:) 

Instance Method

# firstRange(of:)

Finds and returns the range of the first occurrence of a given regex within the collection.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func firstRange(of regex: some RegexComponent) -> Range?
```

Available when `SubSequence` is `Substring`.

## Parameters 

`regex`  

The regex to search for.

## Return Value

A range in the collection of the first occurrence of `regex`. Returns `nil` if `regex` is not found.

