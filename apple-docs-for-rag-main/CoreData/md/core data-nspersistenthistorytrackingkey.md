

- Core Data
-  NSPersistentHistoryTrackingKey 

Global Variable

# NSPersistentHistoryTrackingKey

The key you use to enable persistent history tracking.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
let NSPersistentHistoryTrackingKey: String
```

## Mentioned in 

Consuming relevant store changes

## Discussion

Persistent history tracking is off by default.

## See Also

### Maintaining a record of changes

func currentPersistentHistoryToken(fromStores: [Any]?) -> NSPersistentHistoryToken?

Returns a single persistent history token representing all of the specified stores.

