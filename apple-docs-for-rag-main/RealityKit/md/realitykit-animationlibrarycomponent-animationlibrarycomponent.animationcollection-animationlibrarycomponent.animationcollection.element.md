

- RealityKit
- AnimationLibraryComponent
- AnimationLibraryComponent.AnimationCollection
-  AnimationLibraryComponent.AnimationCollection.Element 

Type Alias

# AnimationLibraryComponent.AnimationCollection.Element

A key-value pair from the collection consisting of the name of an animation and the animation itself.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
typealias Element = (key: String, value: AnimationResource)
```

## See Also

### Accessing animations

subscript(String) -> AnimationResource?

Accesses a single animation in the collection with a key.

subscript(Range&lt;AnimationLibraryComponent.AnimationCollection.Index>) -> AnimationLibraryComponent.AnimationCollection.SubSequence

Accesses animations in the collection within an index range.

subscript(AnimationLibraryComponent.AnimationCollection.Index) -> AnimationLibraryComponent.AnimationCollection.Element

Accesses a single animation in the collection at an index.

typealias SubSequence

A sequence that represents a contiguous subrange of animations in the collection.

