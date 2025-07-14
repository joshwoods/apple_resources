

- RealityKit
- AnimationLibraryComponent
- AnimationLibraryComponent.AnimationCollection
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accesses a single animation in the collection at an index.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
subscript(position: AnimationLibraryComponent.AnimationCollection.Index) -> AnimationLibraryComponent.AnimationCollection.Element { get }
```

## Parameters 

`position`  

An index into the collection’s dictionary.

## Return Value

The animation at the dictionary index.

## See Also

### Accessing animations

subscript(String) -> AnimationResource?

Accesses a single animation in the collection with a key.

subscript(Range&lt;AnimationLibraryComponent.AnimationCollection.Index>) -> AnimationLibraryComponent.AnimationCollection.SubSequence

Accesses animations in the collection within an index range.

typealias SubSequence

A sequence that represents a contiguous subrange of animations in the collection.

typealias Element

A key-value pair from the collection consisting of the name of an animation and the animation itself.

