

- Model I/O
- MDLAsset
-  childObjects(of:) 

Instance Method

# childObjects(of:)

Returns all objects contained in the asset of the specified class.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func childObjects(of objectClass: AnyClass) -> [MDLObject]
```

## Parameters 

`objectClass`  

A Model I/O class (that is, a subclass of MDLObject) representing a type of object stored in the asset. For example, pass the MDLMesh class to find all 3D objects stored in the asset, or the MDLLight class to find all light sources.

## Return Value

An array of objects of the specified type, or an empty array if no such objects exist.

## Discussion

This method searches the asset’s entire child object hierarchy to find all objects of the specified type contained in the asset.

## See Also

### Working with Asset Content

func object(at: Int) -> MDLObject

Returns the top-level object at the specified index in the asset.

subscript(Int) -> MDLObject?

Returns the top-level object at the specified index in the asset, using subscript syntax.

var count: Int

The number of top-level objects in the asset.

func add(MDLObject)

Adds the specified object to the asset’s list of top-level objects.

func remove(MDLObject)

Removes the specified object from the asset’s list of top-level objects.

var boundingBox: MDLAxisAlignedBoundingBox

The minimum region entirely enclosing the asset’s contents.

func boundingBox(atTime: TimeInterval) -> MDLAxisAlignedBoundingBox

Returns the minimum region entirely enclosing the asset’s contents at the specified time sample.

var url: URL?

The URL from which the asset was loaded, if available.

var bufferAllocator: any MDLMeshBufferAllocator

An object responsible for allocating mesh vertex data loaded from the asset.

var vertexDescriptor: MDLVertexDescriptor?

The description of the vertex data format to be used for loading mesh data from the asset.

var masters: any MDLObjectContainerComponent

An array of objects that can be reused in the asset’s object hierarchy through instancing.

Deprecated

