

- System
- FilePath
- FilePath.ComponentView
-  replace(\_:with:maxReplacements:) 

Instance Method

# replace(\_:with:maxReplacements:)

Replaces all occurrences of a target sequence with a given collection

SystemSwiftiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
mutating func replace(
    _ other: C,
    with replacement: Replacement,
    maxReplacements: Int = .max
) where C : Collection, Replacement : Collection, Self.Element == C.Element, C.Element == Replacement.Element
```

Available when `Element` conforms to `Equatable`.

## Parameters 

`other`  

The sequence to replace.

`replacement`  

The new elements to add to the collection.

`maxReplacements`  

A number specifying how many occurrences of `other` to replace. Default is `Int.max`.

