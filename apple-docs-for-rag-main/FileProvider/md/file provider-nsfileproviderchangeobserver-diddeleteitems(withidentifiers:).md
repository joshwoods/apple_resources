

- File Provider
- NSFileProviderChangeObserver
-  didDeleteItems(withIdentifiers:) 

Instance Method

# didDeleteItems(withIdentifiers:)

Tells the observer that the specified items have been deleted.

iOS 11.0+iPadOS 11.0+macOS 11.0+visionOS 1.0+

``` source
func didDeleteItems(withIdentifiers deletedItemIdentifiers: [NSFileProviderItemIdentifier])
```

**Required**

## Parameters 

`deletedItemIdentifiers`  

An array of identifiers for the deleted items.

## See Also

### Observing Changes

func didUpdate([any NSFileProviderItemProtocol])

Tells the observer that the specified items have been updated.

**Required**

func finishEnumeratingChanges(upTo: NSFileProviderSyncAnchor, moreComing: Bool)

Tells the observer that all of the changes have been enumerated up to the specified sync anchor.

**Required**

func finishEnumeratingWithError(any Error)

Tells the observer that an error occurred during change notification.

**Required**

var suggestedBatchSize: Int

The batch size that the system recommends.

