

- Swift
- RangeReplaceableCollection
-  replace(\_:with:maxReplacements:) 

Instance Method

# replace(\_:with:maxReplacements:)

Replaces all occurrences of the sequence matching the given regex with a given collection.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
mutating func replace(
    _ regex: some RegexComponent,
    with replacement: Replacement,
    maxReplacements: Int = .max
) where Replacement : Collection, Replacement.Element == Character
```

Available when `SubSequence` is `Substring`.

## Parameters 

`regex`  

A regex describing the sequence to replace.

`replacement`  

The new elements to add to the collection.

`maxReplacements`  

A number specifying how many occurrences of the sequence matching `regex` to replace. Default is `Int.max`.

