

- RealityKit
- AnimationLibraryComponent
- AnimationLibraryComponent.AnimationCollection
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accesses animations in the collection within an index range.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
subscript(bounds: Range) -> AnimationLibraryComponent.AnimationCollection.SubSequence { get }
```

## Parameters 

`bounds`  

A range of indices to look up.

## Return Value

A subsequence of animation resources in the range of `bounds`.

## See Also

### Accessing animations

subscript(String) -> AnimationResource?

Accesses a single animation in the collection with a key.

subscript(AnimationLibraryComponent.AnimationCollection.Index) -> AnimationLibraryComponent.AnimationCollection.Element

Accesses a single animation in the collection at an index.

typealias SubSequence

A sequence that represents a contiguous subrange of animations in the collection.

typealias Element

A key-value pair from the collection consisting of the name of an animation and the animation itself.

