

- File Provider
-  NSFileProviderChangeObserver 

Protocol

# NSFileProviderChangeObserver

An observer that receives changes and deletions during enumeration.

iOS 11.0+iPadOS 11.0+macOS 11.0+visionOS 1.0+

``` source
protocol NSFileProviderChangeObserver : NSObjectProtocol
```

## Topics

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

func finishEnumeratingWithError(any Error)

Tells the observer that an error occurred during change notification.

**Required**

var suggestedBatchSize: Int

The batch size that the system recommends.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Change Tracking

Tracking Your File Provider’s Changes

Create an enumerator to track changes to your file provider’s content.

struct NSFileProviderSyncAnchor

A synchronization point that represents the last batch of changes returned by the enumerator.

