

- Core Data
- NSCoreDataCoreSpotlightDelegate
-  searchableIndex(\_:reindexAllSearchableItemsWithAcknowledgementHandler:) 

Instance Method

# searchableIndex(\_:reindexAllSearchableItemsWithAcknowledgementHandler:)

Reindexes all searchable items and clears any local state.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
func searchableIndex(
    _ searchableIndex: CSSearchableIndex,
    reindexAllSearchableItemsWithAcknowledgementHandler acknowledgementHandler: @escaping () -> Void
)
```

## Parameters 

`searchableIndex`  

The index that requires reindexing.

`acknowledgementHandler`  

The handler to call when you finish saving client state information.

## Discussion

For more information, see searchableIndex(_:reindexAllSearchableItemsWithAcknowledgementHandler:).

## See Also

### Updating the Index

static let indexDidUpdateNotification: Notification.Name

The notification the delegate posts after Spotlight updates the index.

func searchableIndex(CSSearchableIndex, reindexSearchableItemsWithIdentifiers: [String], acknowledgementHandler: () -> Void)

Reindexes the searchable items for the specified identifiers.

