

- File Provider
-  NSFileProviderEnumerator 

Protocol

# NSFileProviderEnumerator

A protocol for enumerating items and changes.

iOS 11.0+iPadOS 11.0+macOS 11.0+visionOS 1.0+

``` source
protocol NSFileProviderEnumerator : NSObjectProtocol
```

## Mentioned in 

Synchronizing the File Provider Extension

Defining Your File Provider’s Content

## Topics

### Enumerating Items and Changes

func enumerateItems(for: any NSFileProviderEnumerationObserver, startingAt: NSFileProviderPage)

Requests the next batch of items, starting at the specified page.

**Required**

func enumerateChanges(for: any NSFileProviderChangeObserver, from: NSFileProviderSyncAnchor)

Requests the next batch of changes after the specified sync anchor.

func currentSyncAnchor(completionHandler: (NSFileProviderSyncAnchor?) -> Void)

Returns the current sync anchor.

func invalidate()

Stops the enumeration of items and changes.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Inherited By

- NSFileProviderPendingSetEnumerator

