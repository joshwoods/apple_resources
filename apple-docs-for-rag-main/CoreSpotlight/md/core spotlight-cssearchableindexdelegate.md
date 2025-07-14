

- Core Spotlight
-  CSSearchableIndexDelegate 

Protocol

# CSSearchableIndexDelegate

A protocol that defines methods a delegate object or app extension uses to handle communication from the on-device index.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
protocol CSSearchableIndexDelegate : NSObjectProtocol
```

## Mentioned in 

Regenerating your app’s indexes on demand

## Overview

The `CSSearchableIndexDelegate` protocol defines methods that a delegate object or an app extension can use to handle communication from the on-device index. Apps that are long-running or that perform batch updates to the index should implement the required methods of this protocol in either a delegate object or an app extension.

The index delegate methods are called when there is an issue with the index and more information is needed from an app. For example, the methods can be called when the entire index is lost or there was a failure to process data for some identifiers.

## Topics

### Getting item-related details

func data(for: CSSearchableIndex, itemIdentifier: String, typeIdentifier: String) throws -> Data

func fileURL(for: CSSearchableIndex, itemIdentifier: String, typeIdentifier: String, inPlace: Bool) throws -> URL

### Updating the index

func searchableIndex(CSSearchableIndex, reindexAllSearchableItemsWithAcknowledgementHandler: () -> Void)

Tells the delegate to reindex all searchable data and clear all local state information.

**Required**

func searchableIndex(CSSearchableIndex, reindexSearchableItemsWithIdentifiers: [String], acknowledgementHandler: () -> Void)

Tells the delegate to reindex the searchable items associated with the specified identifiers.

**Required**

### Getting information about indexing

func searchableIndexDidThrottle(CSSearchableIndex)

Tells the delegate that indexing is being throttled.

func searchableIndexDidFinishThrottle(CSSearchableIndex)

Tells the delegate that the index throttling has finished.

### Instance Methods

func searchableItems(forIdentifiers: [String], searchableItemsHandler: ([CSSearchableItem]) -> Void)

func searchableItemsDidUpdate([CSSearchableItem])

Tells the delegate that the framework updated the list of searchable items.

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- CSIndexExtensionRequestHandler

## See Also

### Indexes

class CSSearchableIndex

An on-device index for your app’s searchable content.

