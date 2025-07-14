

- RealityKit
- LowLevelMesh
- LowLevelMesh.PartsCollection
-  replaceAll(\_:) 

Instance Method

# replaceAll(\_:)

Replaces all mesh parts in this collection with those from the new sequence.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
mutating func replaceAll(_ newElements: S) where S : Sequence, S.Element == LowLevelMesh.Part
```

## Parameters 

`newElements`  

The elements to replace the contents of the collection.

## See Also

### Updating collection contents

func append(LowLevelMesh.PartsCollection.Element)

Adds an element to the end of the collection.

func append&lt;S>(contentsOf: S)

Adds the elements of a sequence or collection to the end of this collection.

func removeAll()

Removes all mesh parts from this collection.

