

- RealityKit
- MeshInstanceCollection
-  count 

Instance Property

# count

Number of instances.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var count: Int { get }
```

## See Also

### Using the collection

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

subscript(String) -> MeshResource.Instance?

Read an instance given its name.

