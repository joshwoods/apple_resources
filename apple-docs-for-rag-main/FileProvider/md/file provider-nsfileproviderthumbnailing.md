

- File Provider
-  NSFileProviderThumbnailing 

Protocol

# NSFileProviderThumbnailing

Support for item thumbnails.

iOS 16.0+iPadOS 16.0+macOS 11.0+visionOS 1.0+

``` source
protocol NSFileProviderThumbnailing : NSObjectProtocol
```

## Overview

Adopt this protocol if your File Provider extension supports downloading thumbnails from the remote storage.

## Topics

### Providing Thumbnails

func fetchThumbnails(for: [NSFileProviderItemIdentifier], requestedSize: CGSize, perThumbnailCompletionHandler: (NSFileProviderItemIdentifier, Data?, (any Error)?) -> Void, completionHandler: ((any Error)?) -> Void) -> Progress

Asks the file provider for a thumbnail of the specified items.

**Required**

## Relationships

### Inherits From

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

protocol NSFileProviderPendingSetEnumerator

A protocol for enumerating pending items.

