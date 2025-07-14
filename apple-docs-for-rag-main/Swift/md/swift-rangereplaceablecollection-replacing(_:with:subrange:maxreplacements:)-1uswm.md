

- Swift
- RangeReplaceableCollection
-  replacing(\_:with:subrange:maxReplacements:) 

Instance Method

# replacing(\_:with:subrange:maxReplacements:)

Returns a new collection in which all occurrences of a target sequence are replaced by another collection.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func replacing(
    _ other: C,
    with replacement: Replacement,
    subrange: Range,
    maxReplacements: Int = .max
) -> Self where C : Collection, Replacement : Collection, Self.Element == C.Element, C.Element == Replacement.Element
```

Available when `Element` conforms to `Equatable`.

## Parameters 

`other`  

The sequence to replace.

`replacement`  

The new elements to add to the collection.

`subrange`  

The range in the collection in which to search for `other`.

`maxReplacements`  

A number specifying how many occurrences of `other` to replace. Default is `Int.max`.

## Return Value

A new collection in which all occurrences of `other` in `subrange` of the collection are replaced by `replacement`.

