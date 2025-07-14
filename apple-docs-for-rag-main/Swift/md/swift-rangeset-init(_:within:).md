

- Swift
- RangeSet
-  init(\_:within:) 

Initializer

# init(\_:within:)

Creates a new range set containing ranges that contain only the specified indices in the given collection.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
init(
    _ indices: S,
    within collection: C
) where Bound == S.Element, S : Sequence, C : Collection, S.Element == C.Index
```

Available when `Bound` conforms to `Comparable`.

## Parameters 

`collection`  

The collection that contains `index`.

