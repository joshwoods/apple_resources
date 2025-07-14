

- Swift
- JoinedSequence
-  init(base:separator:) 

Initializer

# init(base:separator:)

Creates an iterator that presents the elements of the sequences traversed by `base`, concatenated using `separator`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    base: Base,
    separator: Separator
) where Separator : Sequence, Separator.Element == Base.Element.Element
```

## Discussion

Complexity

O(`separator.count`).

