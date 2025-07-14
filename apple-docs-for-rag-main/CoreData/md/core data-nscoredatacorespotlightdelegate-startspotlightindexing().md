

- Core Data
- NSCoreDataCoreSpotlightDelegate
-  startSpotlightIndexing() 

Instance Method

# startSpotlightIndexing()

Starts the indexing of the store’s entities.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
func startSpotlightIndexing()
```

## Discussion

After you call this method, the delegate posts a notification whenever the index changes. The type of notification is indexDidUpdateNotification, and its `userInfo` dictionary contains the keys NSStoreUUIDKey and NSPersistentHistoryTokenKey.

## See Also

### Managing the Index

func attributeSet(for: NSManagedObject) -> CSSearchableItemAttributeSet?

Returns the searchable attributes for the specified managed object.

func deleteSpotlightIndex(completionHandler: ((any Error)?) -> Void)

Deletes all searchable items from the configured index.

func stopSpotlightIndexing()

Stops the indexing of the store’s entities.

