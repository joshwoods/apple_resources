

- Model I/O
- MDLAsset
-  masters Deprecated

Instance Property

# masters

An array of objects that can be reused in the asset’s object hierarchy through instancing.

iOS 10.0–15.0DeprecatediPadOS 10.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.12–12.0DeprecatedtvOS 10.0–15.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
var masters: any MDLObjectContainerComponent { get set }
```

## Discussion

Some asset formats supported by Model I/O provide *instancing*, a feature where the asset provides a single definition for an object, then can reuse that definition at multiple points in a scene. For example, an asset describing a scene of a table and chairs could contain mesh and material data for only one chair, then use instancing to place several of the same chair around the table.

If an object loaded from an asset is an instance of one of that asset’s primary objects, that object’s instance property refers to the primary object.

## See Also

### Working with Asset Content

func object(at: Int) -> MDLObject

Returns the top-level object at the specified index in the asset.

subscript(Int) -> MDLObject?

Returns the top-level object at the specified index in the asset, using subscript syntax.

var count: Int

The number of top-level objects in the asset.

func childObjects(of: AnyClass) -> [MDLObject]

Returns all objects contained in the asset of the specified class.

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

