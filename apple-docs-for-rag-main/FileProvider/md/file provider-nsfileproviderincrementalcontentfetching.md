

- File Provider
-  NSFileProviderIncrementalContentFetching 

Protocol

# NSFileProviderIncrementalContentFetching

Support for fetching changes to the item’s content.

iOS 16.0+iPadOS 16.0+macOS 11.0+visionOS 1.0+

``` source
protocol NSFileProviderIncrementalContentFetching : NSObjectProtocol
```

## Overview

Adopt this protocol to support the incremental fetching of changes from your remote storage. If you don’t implement the fetchContents(for:version:usingExistingContentsAt:existingVersion:request:completionHandler:) method, the system calls your fetchContents(for:version:request:completionHandler:) method for all updates.

## Topics

### Incrementally Fetching Contents

func fetchContents(for: NSFileProviderItemIdentifier, version: NSFileProviderItemVersion?, usingExistingContentsAt: URL, existingVersion: NSFileProviderItemVersion, request: NSFileProviderRequest, completionHandler: (URL?, NSFileProviderItem?, (any Error)?) -> Void) -> Progress

Asks the file provider for an update of the specified item.

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

protocol NSFileProviderPendingSetEnumerator

A protocol for enumerating pending items.

