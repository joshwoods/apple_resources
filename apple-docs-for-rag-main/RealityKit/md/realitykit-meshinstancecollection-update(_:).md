

- RealityKit
- MeshInstanceCollection
-  update(\_:) 

Instance Method

# update(\_:)

Update an existing instance. The old instance is returned.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
@discardableResult
mutating func update(_ instance: MeshResource.Instance) -> MeshResource.Instance?
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

subscript(String) -> MeshResource.Instance?

Read an instance given its name.

