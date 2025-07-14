

- RealityKit
- AnimationLibraryComponent
- AnimationLibraryComponent.AnimationCollection
-  formIndex(after:) 

Instance Method

# formIndex(after:)

Replaces the index with its successor.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
func formIndex(after i: inout AnimationLibraryComponent.AnimationCollection.Index)
```

## See Also

### Manipulating indices

var startIndex: AnimationLibraryComponent.AnimationCollection.Index

An index to the first animation in the collection.

var endIndex: AnimationLibraryComponent.AnimationCollection.Index

An index to the last animation in the collection.

func index(after: AnimationLibraryComponent.AnimationCollection.Index) -> AnimationLibraryComponent.AnimationCollection.Index

Returns the position in the collection that follows an index.

struct Index

An object that represents a position in the collection.

