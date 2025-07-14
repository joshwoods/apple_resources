

- RealityKit
- AnimationLibraryComponent
- AnimationLibraryComponent.AnimationCollection
-  AnimationLibraryComponent.AnimationCollection.Index 

Structure

# AnimationLibraryComponent.AnimationCollection.Index

An object that represents a position in the collection.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct Index
```

## Topics

### Operators

static func == (AnimationLibraryComponent.AnimationCollection.Index, AnimationLibraryComponent.AnimationCollection.Index) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func &lt; (AnimationLibraryComponent.AnimationCollection.Index, AnimationLibraryComponent.AnimationCollection.Index) -> Bool

Returns a Boolean value that indicates whether the first argument represents a position before the second argument.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Comparable Implementations

Equatable Implementations

## Relationships

### Conforms To

- Comparable
- Equatable
- Hashable
- Sendable

## See Also

### Manipulating indices

var startIndex: AnimationLibraryComponent.AnimationCollection.Index

An index to the first animation in the collection.

var endIndex: AnimationLibraryComponent.AnimationCollection.Index

An index to the last animation in the collection.

func index(after: AnimationLibraryComponent.AnimationCollection.Index) -> AnimationLibraryComponent.AnimationCollection.Index

Returns the position in the collection that follows an index.

func formIndex(after: inout AnimationLibraryComponent.AnimationCollection.Index)

Replaces the index with its successor.

