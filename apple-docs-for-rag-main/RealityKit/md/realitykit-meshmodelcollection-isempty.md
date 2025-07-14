

- RealityKit
- MeshModelCollection
-  isEmpty 

Instance Property

# isEmpty

True if there are no models.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var isEmpty: Bool { get }
```

## See Also

### Using the collection

var count: Int

Number of models.

func insert(MeshResource.Model) -> Bool

Add a new model to the container. Returns true if added.

func remove(id: String) -> MeshResource.Model?

Remove a model by id.

func removeAll()

Remove all the models.

func update(MeshResource.Model) -> MeshResource.Model?

Update an existing model. The old model is returned.

subscript(String) -> MeshResource.Model?

Read a model given its id.

