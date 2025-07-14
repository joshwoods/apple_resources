

- RealityKit
- MeshPartCollection
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Read a part given its id.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
subscript(id: String) -> MeshResource.Part? { get }
```

## See Also

### Using the collection

var count: Int

Number of parts.

var isEmpty: Bool

True if there are no parts.

func insert(MeshResource.Part) -> Bool

Add a new part to the container. Returns true if added.

func remove(id: String) -> MeshResource.Part?

Remove a part by id.

func removeAll()

Remove all the parts.

func update(MeshResource.Part) -> MeshResource.Part?

Update an existing part. The old part is returned.

