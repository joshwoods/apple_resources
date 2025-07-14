

- Core Data
- NSCoreDataCoreSpotlightDelegate
-  searchableIndex(\_:reindexSearchableItemsWithIdentifiers:acknowledgementHandler:) 

Instance Method

# searchableIndex(\_:reindexSearchableItemsWithIdentifiers:acknowledgementHandler:)

Reindexes the searchable items for the specified identifiers.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
func searchableIndex(
    _ searchableIndex: CSSearchableIndex,
    reindexSearchableItemsWithIdentifiers identifiers: [String],
    acknowledgementHandler: @escaping () -> Void
)
```

## Parameters 

`searchableIndex`  

The index that contains the items that require reindexing.

`identifiers`  

An array of strings that identify the searchable items.

`acknowledgementHandler`  

The handler to call when you finish saving client state information.

## Discussion

For more information, see searchableIndex(_:reindexSearchableItemsWithIdentifiers:acknowledgementHandler:).

## See Also

### Updating the Index

static let indexDidUpdateNotification: Notification.Name

The notification the delegate posts after Spotlight updates the index.

func searchableIndex(CSSearchableIndex, reindexAllSearchableItemsWithAcknowledgementHandler: () -> Void)

Reindexes all searchable items and clears any local state.

