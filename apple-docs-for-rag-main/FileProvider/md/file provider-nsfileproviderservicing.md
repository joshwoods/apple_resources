

- File Provider
-  NSFileProviderServicing 

Protocol

# NSFileProviderServicing

Support for providing a custom service source.

iOS 16.0+iPadOS 16.0+macOS 11.0+visionOS 1.0+

``` source
protocol NSFileProviderServicing : NSObjectProtocol
```

## Overview

Adopt this protocol if your File Provider extension supports custom services. For more information on custom services, see NSFileProviderService.

## Topics

### Providing a Service Source

func supportedServiceSources(for: NSFileProviderItemIdentifier, completionHandler: ([any NSFileProviderServiceSource]?, (any Error)?) -> Void) -> Progress

Asks the File Provider extension for an array of custom communication channels.

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

protocol NSFileProviderCustomAction

Support for custom actions.

struct NSFileProviderExtensionActionIdentifier

An identifier for custom actions.

protocol NSFileProviderThumbnailing

Support for item thumbnails.

protocol NSFileProviderPendingSetEnumerator

A protocol for enumerating pending items.

