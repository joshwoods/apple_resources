

- RealityKit
- AnimationLibraryComponent
- AnimationLibraryComponent.AnimationCollection
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accesses a single animation in the collection with a key.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
subscript(key: String) -> AnimationResource? { get set }
```

## Parameters 

`key`  

A name for the animation to look up.

## Return Value

An animation resource, or `nil` if the component can’t find one that maps to the `key`.

## See Also

### Accessing animations

subscript(Range&lt;AnimationLibraryComponent.AnimationCollection.Index>) -> AnimationLibraryComponent.AnimationCollection.SubSequence

Accesses animations in the collection within an index range.

subscript(AnimationLibraryComponent.AnimationCollection.Index) -> AnimationLibraryComponent.AnimationCollection.Element

Accesses a single animation in the collection at an index.

typealias SubSequence

A sequence that represents a contiguous subrange of animations in the collection.

typealias Element

A key-value pair from the collection consisting of the name of an animation and the animation itself.

