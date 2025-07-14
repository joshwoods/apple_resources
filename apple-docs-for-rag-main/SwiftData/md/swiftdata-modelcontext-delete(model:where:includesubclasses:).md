

- SwiftData
- ModelContext
-  delete(model:where:includeSubclasses:) 

Instance Method

# delete(model:where:includeSubclasses:)

Removes each model satisfying the given predicate from the persistent storage during the next save operation.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Swift 5.9+

``` source
func delete(
    model: T.Type,
    where predicate: Predicate? = nil,
    includeSubclasses: Bool = true
) throws where T : PersistentModel
```

## Parameters 

`model`  

The type of the model to remove.

`predicate`  

The logical condition to use when determining if the context should remove a particular model. The default value is `nil`.

`includeSubclasses`  

A Boolean value that indicates whether the context includes subclasses of the specified model type when evaluating models to remove. The default value is `true`.

## Discussion

Warning

If you don’t provide a predicate, the context will remove all models of the specified type from the persistent storage.

## See Also

### Deleting models

var deletedModelsArray: [any PersistentModel]

The array of registered models that the context will remove from the persistent storage during the next save operation.

func delete&lt;T>(T)

Removes the specified model from the persistent storage during the next save operation.

