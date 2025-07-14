

- RealityKit
- MeshInstanceCollection
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Read an instance given its name.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
subscript(id: String) -> MeshResource.Instance? { get }
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

func removeAll()

Remove all the instances.

func update(MeshResource.Instance) -> MeshResource.Instance?

Update an existing instance. The old instance is returned.

