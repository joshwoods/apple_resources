

- MusicKit
- MusicItemCollection
-  split(separator:maxSplits:omittingEmptySubsequences:) 

Instance Method

# split(separator:maxSplits:omittingEmptySubsequences:)

Returns the longest possible subsequences of the collection, in order, around elements equal to the given separator.

MusicKitSwiftiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func split(
    separator: C,
    maxSplits: Int = .max,
    omittingEmptySubsequences: Bool = true
) -> [Self.SubSequence] where C : Collection, Self.Element == C.Element
```

Available when `Element` conforms to `Equatable`.

## Parameters 

`separator`  

The element to be split upon.

## Return Value

A collection of subsequences, split from this collection’s elements.

