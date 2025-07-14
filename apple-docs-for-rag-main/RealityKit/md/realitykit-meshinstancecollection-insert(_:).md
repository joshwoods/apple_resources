

- RealityKit
- MeshInstanceCollection
-  insert(\_:) 

Instance Method

# insert(\_:)

Add a new instance to the container. Returns true if added.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
@discardableResult
mutating func insert(_ instance: MeshResource.Instance) -> Bool
```

## See Also

### Using the collection

var count: Int

Number of instances.

var isEmpty: Bool

True if there are no instances.

func remove(id: String) -> MeshResource.Instance?

Remove an instance by name.

func removeAll()

Remove all the instances.

func update(MeshResource.Instance) -> MeshResource.Instance?

Update an existing instance. The old instance is returned.

subscript(String) -> MeshResource.Instance?

Read an instance given its name.

