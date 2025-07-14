

- Core Data
- NSPersistentStoreCoordinator
-  currentPersistentHistoryToken(fromStores:) 

Instance Method

# currentPersistentHistoryToken(fromStores:)

Returns a single persistent history token representing all of the specified stores.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
func currentPersistentHistoryToken(fromStores stores: [Any]?) -> NSPersistentHistoryToken?
```

## Parameters 

`stores`  

The persistent stores of interest.

## Return Value

A persistent history token, or `nil` if the coordinator can’t create one.

## Discussion

If you specify `nil` or provide an empty array, the coordinator attempts to create a token for all of its registered stores.

## See Also

### Maintaining a record of changes

let NSPersistentHistoryTrackingKey: String

The key you use to enable persistent history tracking.

