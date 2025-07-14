

- SwiftData
-  DataStoreBatchDeleteRequest 

Structure

# DataStoreBatchDeleteRequest

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+Swift 5.9+

``` source
struct DataStoreBatchDeleteRequest where T : PersistentModel
```

## Topics

### Instance Properties

let editingState: EditingState

let predicate: Predicate&lt;T>?

## Relationships

### Conforms To

- Sendable

## See Also

### Deleting persisted model data

func delete&lt;T>(DataStoreBatchDeleteRequest&lt;T>) throws

**Required**

