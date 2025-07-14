

- Core Data
- NSCoreDataCoreSpotlightDelegate
-  stopSpotlightIndexing() 

Instance Method

# stopSpotlightIndexing()

Stops the indexing of the store’s entities.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
func stopSpotlightIndexing()
```

## Discussion

After you call this method, the delegate no longer posts notifications about index changes.

## See Also

### Managing the Index

func attributeSet(for: NSManagedObject) -> CSSearchableItemAttributeSet?

Returns the searchable attributes for the specified managed object.

func deleteSpotlightIndex(completionHandler: ((any Error)?) -> Void)

Deletes all searchable items from the configured index.

func startSpotlightIndexing()

Starts the indexing of the store’s entities.

