

- Core Data
-  NSCoreDataCoreSpotlightDelegate 

Class

# NSCoreDataCoreSpotlightDelegate

A set of methods that enable integration with Core Spotlight.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
class NSCoreDataCoreSpotlightDelegate
```

## Overview

Note

Core Spotlight integration is only available for persistent stores that have a store type of sqlite, and which use persistent history tracking. For more information, see Consuming relevant store changes.

## Topics

### Creating a Core Spotlight Delegate

init(forStoreWith: NSPersistentStoreDescription, coordinator: NSPersistentStoreCoordinator)

Creates a Core Spotlight delegate with the specified store description and coordinator.

convenience init(forStoreWith: NSPersistentStoreDescription, model: NSManagedObjectModel)

Creates a Core Spotlight delegate with the specified store description and managed object model.

Deprecated

### Configuring the Index

var isIndexingEnabled: Bool

A Boolean value that indicates whether Core Data is currently updating the Core Spotlight index with the persistent store’s entities.

func domainIdentifier() -> String

Returns the domain identifier.

func indexName() -> String?

Returns the index’s name.

### Managing the Index

func attributeSet(for: NSManagedObject) -> CSSearchableItemAttributeSet?

Returns the searchable attributes for the specified managed object.

func deleteSpotlightIndex(completionHandler: ((any Error)?) -> Void)

Deletes all searchable items from the configured index.

func startSpotlightIndexing()

Starts the indexing of the store’s entities.

func stopSpotlightIndexing()

Stops the indexing of the store’s entities.

### Updating the Index

static let indexDidUpdateNotification: Notification.Name

The notification the delegate posts after Spotlight updates the index.

func searchableIndex(CSSearchableIndex, reindexAllSearchableItemsWithAcknowledgementHandler: () -> Void)

Reindexes all searchable items and clears any local state.

func searchableIndex(CSSearchableIndex, reindexSearchableItemsWithIdentifiers: [String], acknowledgementHandler: () -> Void)

Reindexes the searchable items for the specified identifiers.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Integrating with Spotlight

let NSCoreDataCoreSpotlightExporter: String

The key you use to specify your Core Spotlight delegate.

Spotlight record keys

The keys for the values that exist in Spotlight’s external record files.

Showcase App Data in Spotlight

Index app data so users can find it by using Spotlight search.

