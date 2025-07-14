

- Model I/O
- MDLAsset
-  url 

Instance Property

# url

The URL from which the asset was loaded, if available.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var url: URL? { get }
```

## Discussion

For assets created from a URL (with the init(url:) or init(url:vertexDescriptor:bufferAllocator:) initializer), this property is the URL that the asset was loaded from. For assets created manually, this property’s value is `nil`.

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

var bufferAllocator: any MDLMeshBufferAllocator

An object responsible for allocating mesh vertex data loaded from the asset.

var vertexDescriptor: MDLVertexDescriptor?

The description of the vertex data format to be used for loading mesh data from the asset.

var masters: any MDLObjectContainerComponent

An array of objects that can be reused in the asset’s object hierarchy through instancing.

Deprecated

