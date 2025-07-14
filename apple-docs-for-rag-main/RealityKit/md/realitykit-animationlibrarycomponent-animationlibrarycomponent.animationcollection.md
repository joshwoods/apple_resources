

- RealityKit
- AnimationLibraryComponent
-  AnimationLibraryComponent.AnimationCollection 

Structure

# AnimationLibraryComponent.AnimationCollection

A collection of animations an entity can play.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct AnimationCollection
```

## Overview

You use `AnimationCollection` to access animations in an AnimationLibraryComponent.

The initializers for AnimationLibraryComponent create an `AnimationCollection`, so you don’t need to create one directly. You can access the collection with the animations property.

## Topics

### Creating an animation collection

init(dictionaryLiteral: (String, AnimationResource)...)

Creates an animation collection from a dictionary literal.

### Inspecting an animation collection

var count: Int

The number of animations in the collection.

var isEmpty: Bool

A Boolean value that indicates whether the collection is empty.

### Accessing animations

subscript(String) -> AnimationResource?

Accesses a single animation in the collection with a key.

subscript(Range&lt;AnimationLibraryComponent.AnimationCollection.Index>) -> AnimationLibraryComponent.AnimationCollection.SubSequence

Accesses animations in the collection within an index range.

subscript(AnimationLibraryComponent.AnimationCollection.Index) -> AnimationLibraryComponent.AnimationCollection.Element

Accesses a single animation in the collection at an index.

typealias SubSequence

A sequence that represents a contiguous subrange of animations in the collection.

typealias Element

A key-value pair from the collection consisting of the name of an animation and the animation itself.

### Manipulating indices

var startIndex: AnimationLibraryComponent.AnimationCollection.Index

An index to the first animation in the collection.

var endIndex: AnimationLibraryComponent.AnimationCollection.Index

An index to the last animation in the collection.

func index(after: AnimationLibraryComponent.AnimationCollection.Index) -> AnimationLibraryComponent.AnimationCollection.Index

Returns the position in the collection that follows an index.

func formIndex(after: inout AnimationLibraryComponent.AnimationCollection.Index)

Replaces the index with its successor.

struct Index

An object that represents a position in the collection.

### Iterating over animations

func makeIterator() -> AnimationLibraryComponent.AnimationCollection.Iterator

Returns an iterator over the animations in the collection.

struct Iterator

An object to iterate over all animations in the collection.

### Type Aliases

typealias Indices

A type that represents the indices that are valid for subscripting the collection, in ascending order.

### Default Implementations

Collection Implementations

Sequence Implementations

## Relationships

### Conforms To

- Collection
- Sequence

## See Also

### Animation playback

class AnimationResource

An animation for the properties of scenes or entities.

struct AnimationLibraryComponent

A component that represents a collection of animations that an entity can play.

enum AnimationEvents

Notable milestones that the framework signals during animation playback.

class AnimationPlaybackController

A controller that manages animation playback.

enum AnimationRepeatMode

Options that determine whether an animation replays after completion.

