

- RealityKit
- MeshModelCollection
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Read a model given its id.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
subscript(id: String) -> MeshResource.Model? { get }
```

## See Also

### Using the collection

var count: Int

Number of models.

var isEmpty: Bool

True if there are no models.

func insert(MeshResource.Model) -> Bool

Add a new model to the container. Returns true if added.

func remove(id: String) -> MeshResource.Model?

Remove a model by id.

func removeAll()

Remove all the models.

func update(MeshResource.Model) -> MeshResource.Model?

Update an existing model. The old model is returned.

