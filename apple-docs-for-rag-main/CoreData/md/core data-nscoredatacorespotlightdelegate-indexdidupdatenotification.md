

- Core Data
- NSCoreDataCoreSpotlightDelegate
-  indexDidUpdateNotification 

Type Property

# indexDidUpdateNotification

The notification the delegate posts after Spotlight updates the index.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+visionOS

``` source
static let indexDidUpdateNotification: Notification.Name
```

## Discussion

The notification’s `userInfo` dictionary contains the keys NSStoreUUIDKey and NSPersistentHistoryTokenKey.

## See Also

### Updating the Index

func searchableIndex(CSSearchableIndex, reindexAllSearchableItemsWithAcknowledgementHandler: () -> Void)

Reindexes all searchable items and clears any local state.

func searchableIndex(CSSearchableIndex, reindexSearchableItemsWithIdentifiers: [String], acknowledgementHandler: () -> Void)

Reindexes the searchable items for the specified identifiers.

