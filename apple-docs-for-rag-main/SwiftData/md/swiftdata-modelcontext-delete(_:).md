

- SwiftData
- ModelContext
-  delete(\_:) 

Instance Method

# delete(\_:)

Removes the specified model from the persistent storage during the next save operation.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Swift 5.9+

``` source
func delete(_ model: T) where T : PersistentModel
```

## Parameters 

`model`  

The persistent model to delete.

## Discussion

When the context nexts commits its changes, SwiftData removes the model from the persistent storage. If the model is new and in an unsaved state, the context simply discards it.

## See Also

### Deleting models

var deletedModelsArray: [any PersistentModel]

The array of registered models that the context will remove from the persistent storage during the next save operation.

func delete&lt;T>(model: T.Type, where: Predicate&lt;T>?, includeSubclasses: Bool) throws

Removes each model satisfying the given predicate from the persistent storage during the next save operation.

