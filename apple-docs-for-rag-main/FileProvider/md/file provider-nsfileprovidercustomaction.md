

- File Provider
-  NSFileProviderCustomAction 

Protocol

# NSFileProviderCustomAction

Support for custom actions.

iOS 16.0+iPadOS 16.0+macOS 11.0+visionOS 1.0+

``` source
protocol NSFileProviderCustomAction : NSObjectProtocol
```

## Overview

Adopt this protocol to add a custom action to the context menu (for example, when the user control-clicks an item in Finder).

If you want to create an action that displays custom user interface elements, add actions using the File Provider UI framework instead. For more information, see `Adding Actions to the Context Menu`.

## Topics

### Performing Custom Actions

func performAction(identifier: NSFileProviderExtensionActionIdentifier, onItemsWithIdentifiers: [NSFileProviderItemIdentifier], completionHandler: ((any Error)?) -> Void) -> Progress

Tells the File Provider extension to perform a custom action.

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

struct NSFileProviderExtensionActionIdentifier

An identifier for custom actions.

protocol NSFileProviderThumbnailing

Support for item thumbnails.

protocol NSFileProviderPendingSetEnumerator

A protocol for enumerating pending items.

