

- File Provider
- NSFileProviderChangeObserver
-  finishEnumeratingChanges(upTo:moreComing:) 

Instance Method

# finishEnumeratingChanges(upTo:moreComing:)

Tells the observer that all of the changes have been enumerated up to the specified sync anchor.

iOS 11.0+iPadOS 11.0+macOS 11.0+visionOS 1.0+

``` source
func finishEnumeratingChanges(
    upTo anchor: NSFileProviderSyncAnchor,
    moreComing: Bool
)
```

**Required**

## Parameters 

`anchor`  

An object used to identify the end of the current batch of changes.

`moreComing`  

A Boolean value that indicates the file provider still has one or more batches of pending changes.

## See Also

### Observing Changes

func didDeleteItems(withIdentifiers: [NSFileProviderItemIdentifier])

Tells the observer that the specified items have been deleted.

**Required**

func didUpdate([any NSFileProviderItemProtocol])

Tells the observer that the specified items have been updated.

**Required**

func finishEnumeratingWithError(any Error)

Tells the observer that an error occurred during change notification.

**Required**

var suggestedBatchSize: Int

The batch size that the system recommends.

