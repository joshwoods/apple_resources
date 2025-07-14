

- Swift
- RangeReplaceableCollection
-  replacing(with:subrange:maxReplacements:content:) 

Instance Method

# replacing(with:subrange:maxReplacements:content:)

Returns a new collection in which all matches for the regex are replaced, using the given closure to create the regex.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func replacing(
    with replacement: Replacement,
    subrange: Range,
    maxReplacements: Int = .max,
    @RegexComponentBuilder content: () -> some RegexComponent
) -> Self where Replacement : Collection, Replacement.Element == Character
```

Available when `Self` conforms to `BidirectionalCollection` and `SubSequence` is `Substring`.

## Parameters 

`replacement`  

The new elements to add to the collection in place of each match for the regex, using `content` to create the regex.

`subrange`  

The range in the collection in which to search for the regex.

`maxReplacements`  

A number specifying how many occurrences of the regex to replace.

`content`  

A closure that returns the collection to search for and replace.

## Return Value

A new collection in which all matches for regex in `subrange` are replaced by `replacement`, using `content` to create the regex.

