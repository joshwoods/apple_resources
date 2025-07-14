

- RealityKit
- AnimationLibraryComponent
- AnimationLibraryComponent.AnimationCollection
-  index(after:) 

Instance Method

# index(after:)

Returns the position in the collection that follows an index.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
func index(after i: AnimationLibraryComponent.AnimationCollection.Index) -> AnimationLibraryComponent.AnimationCollection.Index
```

## Parameters 

`i`  

A valid index of the collection. `i` must be less than `endIndex`.

## See Also

### Manipulating indices

var startIndex: AnimationLibraryComponent.AnimationCollection.Index

An index to the first animation in the collection.

var endIndex: AnimationLibraryComponent.AnimationCollection.Index

An index to the last animation in the collection.

func formIndex(after: inout AnimationLibraryComponent.AnimationCollection.Index)

Replaces the index with its successor.

struct Index

An object that represents a position in the collection.

