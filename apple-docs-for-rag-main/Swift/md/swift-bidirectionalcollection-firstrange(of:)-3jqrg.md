

- Swift
- BidirectionalCollection
-  firstRange(of:) 

Instance Method

# firstRange(of:)

Returns the range of the first match for the regex within this collection, where the regex is created by the given closure.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func firstRange(@RegexComponentBuilder of content: () -> some RegexComponent) -> Range?
```

Available when `SubSequence` is `Substring`.

## Parameters 

`content`  

A closure that returns a regex to search for.

## Return Value

A range in the collection of the first occurrence of the first match of if the regex returned by `content`. Returns `nil` if no match for the regex is found.

