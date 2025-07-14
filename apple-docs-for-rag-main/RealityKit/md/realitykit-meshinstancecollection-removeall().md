

- RealityKit
- MeshInstanceCollection
-  removeAll() 

Instance Method

# removeAll()

Remove all the instances.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
mutating func removeAll()
```

## See Also

### Using the collection

var count: Int

Number of instances.

var isEmpty: Bool

True if there are no instances.

func insert(MeshResource.Instance) -> Bool

Add a new instance to the container. Returns true if added.

func remove(id: String) -> MeshResource.Instance?

Remove an instance by name.

func update(MeshResource.Instance) -> MeshResource.Instance?

Update an existing instance. The old instance is returned.

subscript(String) -> MeshResource.Instance?

Read an instance given its name.

