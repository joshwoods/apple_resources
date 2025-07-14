

- Core Data
-  NSStagedMigrationManager 

Class

# NSStagedMigrationManager

An object that handles the migration event loop and provides access to the migrating persistent store.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
class NSStagedMigrationManager
```

## Overview

A staged migration manager contains the individual stages of a migration and applies those stages, in the order you specify, when that migration runs. The manager handles the migration’s event loop, and provides access to the migrating store through its container property. Stages can be custom, which enables you to perform tasks immediately before and after a stage runs, or lightweight, which supplements custom stages with those that Core Data can invoke automatically because they’re already compatible with lightweight migrations.

Use NSPersistentStoreStagedMigrationManagerOptionKey to include an instance of NSStagedMigrationManager in your persistent store’s options dictionary, as the following example shows:

```
// Create a migration manager with the required stages.
let manager = NSStagedMigrationManager(stages)

let options = [
    // Enable lightweight migrations for this store.
    NSMigratePersistentStoresAutomaticallyOption: true,
    NSInferMappingModelAutomaticallyOption: true
    // Specify the migration manager to use with this store.
    NSPersistentStoreStagedMigrationManagerOptionKey: manager 
]

// Add the store to the persistent store coordinator.        
let store = coordinator.addPersistentStore(
    type: .sqlite,
    at: storeURL,
    options: options
)
```

## Topics

### Creating a migration manager

convenience init([NSMigrationStage])

Creates a migration manager with the specified stages.

### Accessing the persistent container

var container: NSPersistentContainer?

The container that provides access to the migrating persistent store.

### Accessing the stages

var stages: [NSMigrationStage]

The migration stages.

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

### Migration staging

let NSPersistentStoreStagedMigrationManagerOptionKey: String

The key for specifying your staged migration manager.

