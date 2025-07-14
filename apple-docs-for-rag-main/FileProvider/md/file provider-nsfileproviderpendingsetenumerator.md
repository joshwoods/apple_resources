

- File Provider
-  NSFileProviderPendingSetEnumerator 

Protocol

# NSFileProviderPendingSetEnumerator

A protocol for enumerating pending items.

iOS 16.0+iPadOS 16.0+macOS 11.3+visionOS 1.0+

``` source
protocol NSFileProviderPendingSetEnumerator : NSFileProviderEnumerator
```

## Overview

Items are pending when they’ve changed but the File Provider extension hasn’t yet synced the changes. Examples include local changes that the extension hasn’t uploaded to its remote storage and items that the extension has marked as changed in the working set but hasn’t yet downloaded. The system calls pendingItemsDidChange(completionHandler:) and posts a NSFileProviderPendingSetDidChange notification whenever the set of pending items changes.

To enumerate items in the pending set, call the enumeratorForPendingItems() method, which returns an object that adopts the NSFileProviderPendingSetEnumerator protocol.

The pending enumerator lists the items that meet all of the following criteria:

- The system observed a change, either on disk or in the working set.

- The change occurred more than one second ago.

- The File Provider extension hasn’t yet synced the change with its remote storage.

An item can appear in the pending set for many different reasons, including:

- The system is under load and can’t process all the events in a timely manner.

- The system is performing a long-running operation on the item, such as downloading or uploading new content.

- Pending changes to the item have raised an error.

The pending set only contains items that are already known to the File Provider extension and that remain queued for change longer than the system’s refresh interval. A new file in the local storage won’t appear in the pending set, even if the upload to the remote storage takes several minutes to complete.

## Topics

### Accessing Refresh Data

var domainVersion: NSFileProviderDomainVersion?

The domain version when the system last refreshed the pending set.

**Required**

var refreshInterval: TimeInterval

The amount of time, in seconds, between updates to the pending set.

**Required**

### Instance Properties

var isMaximumSizeReached: Bool

**Required**

## Relationships

### Inherits From

- NSFileProviderEnumerator
- NSObjectProtocol

## See Also

### File Provider protocols

protocol NSFileProviderReplicatedExtension

A File Provider extension in which the system replicates the contents on disk.

protocol NSFileProviderEnumerating

Support for enumerating the file provider’s contents.

protocol NSFileProviderIncrementalContentFetching

Support for fetching changes to the item’s content.

protocol NSFileProviderPartialContentFetching

Support for fetching part of a file’s content.

protocol NSFileProviderServicing

Support for providing a custom service source.

protocol NSFileProviderCustomAction

Support for custom actions.

struct NSFileProviderExtensionActionIdentifier

An identifier for custom actions.

protocol NSFileProviderThumbnailing

Support for item thumbnails.

