

- File Provider
- NSFileProviderChangeObserver
-  didUpdate(\_:) 

Instance Method

# didUpdate(\_:)

Tells the observer that the specified items have been updated.

iOS 11.0+iPadOS 11.0+macOS 11.0+visionOS 1.0+

``` source
func didUpdate(_ updatedItems: [any NSFileProviderItemProtocol])
```

**Required**

## Parameters 

`updatedItems`  

An array of updated items.

## See Also

### Observing Changes

func didDeleteItems(withIdentifiers: [NSFileProviderItemIdentifier])

Tells the observer that the specified items have been deleted.

**Required**

func finishEnumeratingChanges(upTo: NSFileProviderSyncAnchor, moreComing: Bool)

Tells the observer that all of the changes have been enumerated up to the specified sync anchor.

**Required**

func finishEnumeratingWithError(any Error)

Tells the observer that an error occurred during change notification.

**Required**

var suggestedBatchSize: Int

The batch size that the system recommends.

