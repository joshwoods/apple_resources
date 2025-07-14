

- RealityKit
- MeshModelCollection
-  remove(id:) 

Instance Method

# remove(id:)

Remove a model by id.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
@discardableResult
mutating func remove(id: String) -> MeshResource.Model?
```

## See Also

### Using the collection

var count: Int

Number of models.

var isEmpty: Bool

True if there are no models.

func insert(MeshResource.Model) -> Bool

Add a new model to the container. Returns true if added.

func removeAll()

Remove all the models.

func update(MeshResource.Model) -> MeshResource.Model?

Update an existing model. The old model is returned.

subscript(String) -> MeshResource.Model?

Read a model given its id.

