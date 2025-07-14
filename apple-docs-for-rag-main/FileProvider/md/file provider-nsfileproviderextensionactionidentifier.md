

- File Provider
-  NSFileProviderExtensionActionIdentifier 

Structure

# NSFileProviderExtensionActionIdentifier

An identifier for custom actions.

iOS 11.0+iPadOS 11.0+macOS 11.0+visionOS 1.0+

``` source
struct NSFileProviderExtensionActionIdentifier
```

## Topics

### Creating Identifiers

init(String)

Creates a new identifier from the provided string.

init(rawValue: String)

Creates a new identifier from the provided value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

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

protocol NSFileProviderThumbnailing

Support for item thumbnails.

protocol NSFileProviderPendingSetEnumerator

A protocol for enumerating pending items.

