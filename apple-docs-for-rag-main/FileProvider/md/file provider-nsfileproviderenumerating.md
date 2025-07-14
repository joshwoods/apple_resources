

- File Provider
-  NSFileProviderEnumerating 

Protocol

# NSFileProviderEnumerating

Support for enumerating the file provider’s contents.

iOS 16.0+iPadOS 16.0+macOS 11.0+visionOS 1.0+

``` source
protocol NSFileProviderEnumerating : NSObjectProtocol
```

## Topics

### Accessing Enumerators

func enumerator(for: NSFileProviderItemIdentifier, request: NSFileProviderRequest) throws -> any NSFileProviderEnumerator

Tells the file provider to return an enumerator for the provided directory.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Inherited By

- NSFileProviderReplicatedExtension

## See Also

### File Provider protocols

protocol NSFileProviderReplicatedExtension

A File Provider extension in which the system replicates the contents on disk.

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

protocol NSFileProviderPendingSetEnumerator

A protocol for enumerating pending items.

