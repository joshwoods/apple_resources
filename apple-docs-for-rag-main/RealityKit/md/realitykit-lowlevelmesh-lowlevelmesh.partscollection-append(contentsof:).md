

- RealityKit
- LowLevelMesh
- LowLevelMesh.PartsCollection
-  append(contentsOf:) 

Instance Method

# append(contentsOf:)

Adds the elements of a sequence or collection to the end of this collection.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
mutating func append(contentsOf newElements: S) where S : Sequence, S.Element == LowLevelMesh.Part
```

## Parameters 

`newElements`  

The elements to append to the collection.

## See Also

### Updating collection contents

func append(LowLevelMesh.PartsCollection.Element)

Adds an element to the end of the collection.

func replaceAll&lt;S>(S)

Replaces all mesh parts in this collection with those from the new sequence.

func removeAll()

Removes all mesh parts from this collection.

