

- File Provider
- NSFileProviderChangeObserver
-  finishEnumeratingWithError(\_:) 

Instance Method

# finishEnumeratingWithError(\_:)

Tells the observer that an error occurred during change notification.

iOS 11.0+iPadOS 11.0+macOS 11.0+visionOS 1.0+

``` source
func finishEnumeratingWithError(_ error: any Error)
```

**Required**

## Parameters 

`error`  

An object that contains information about the error.

## See Also

### Observing Changes

func didDeleteItems(withIdentifiers: [NSFileProviderItemIdentifier])

Tells the observer that the specified items have been deleted.

**Required**

func didUpdate([any NSFileProviderItemProtocol])

Tells the observer that the specified items have been updated.

**Required**

func finishEnumeratingChanges(upTo: NSFileProviderSyncAnchor, moreComing: Bool)

Tells the observer that all of the changes have been enumerated up to the specified sync anchor.

**Required**

var suggestedBatchSize: Int

The batch size that the system recommends.

