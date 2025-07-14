

- SwiftData
- ModelContext
-  deletedModelsArray 

Instance Property

# deletedModelsArray

The array of registered models that the context will remove from the persistent storage during the next save operation.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Swift 5.9+

``` source
var deletedModelsArray: [any PersistentModel] { get }
```

## See Also

### Deleting models

func delete&lt;T>(T)

Removes the specified model from the persistent storage during the next save operation.

func delete&lt;T>(model: T.Type, where: Predicate&lt;T>?, includeSubclasses: Bool) throws

Removes each model satisfying the given predicate from the persistent storage during the next save operation.

