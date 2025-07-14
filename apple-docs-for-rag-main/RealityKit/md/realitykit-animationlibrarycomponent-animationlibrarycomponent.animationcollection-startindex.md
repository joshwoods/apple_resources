

- RealityKit
- AnimationLibraryComponent
- AnimationLibraryComponent.AnimationCollection
-  startIndex 

Instance Property

# startIndex

An index to the first animation in the collection.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var startIndex: AnimationLibraryComponent.AnimationCollection.Index { get }
```

## See Also

### Manipulating indices

var endIndex: AnimationLibraryComponent.AnimationCollection.Index

An index to the last animation in the collection.

func index(after: AnimationLibraryComponent.AnimationCollection.Index) -> AnimationLibraryComponent.AnimationCollection.Index

Returns the position in the collection that follows an index.

func formIndex(after: inout AnimationLibraryComponent.AnimationCollection.Index)

Replaces the index with its successor.

struct Index

An object that represents a position in the collection.

