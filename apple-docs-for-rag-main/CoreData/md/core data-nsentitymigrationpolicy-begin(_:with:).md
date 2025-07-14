

- Core Data
- NSEntityMigrationPolicy
-  begin(\_:with:) 

Instance Method

# begin(\_:with:)

Sets up state information before the start of a given entity mapping.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func begin(
    _ mapping: NSEntityMapping,
    with manager: NSMigrationManager
) throws
```

## Parameters 

`mapping`  

The mapping object in use.

`manager`  

The migration manager performing the migration.

## Discussion

This method is the precursor to the creation stage. In a custom class, you can implement this method to set up any state information that will be useful for the duration of the migration.

## See Also

### Related Documentation

Core Data Model Versioning and Data Migration Programming Guide

### Customizing Stages of the Mapping Life Cycle

func createDestinationInstances(forSource: NSManagedObject, in: NSEntityMapping, manager: NSMigrationManager) throws

Creates the destination instance(s) for a given source instance.

func endInstanceCreation(forMapping: NSEntityMapping, manager: NSMigrationManager) throws

Indicates the end of the instance creation stage for the specified entity mapping, and the precursor to the next migration stage.

func createRelationships(forDestination: NSManagedObject, in: NSEntityMapping, manager: NSMigrationManager) throws

Constructs the relationships between the newly-created destination instances.

func endRelationshipCreation(forMapping: NSEntityMapping, manager: NSMigrationManager) throws

Indicates the end of the relationship creation stage for the specified entity mapping.

func performCustomValidation(forMapping: NSEntityMapping, manager: NSMigrationManager) throws

Provides the option to perform custom validation on migrated objects during the validation stage of the entity migration policy.

func end(NSEntityMapping, manager: NSMigrationManager) throws

Performs cleanup at the end of the migration, from any phase of the mapping.

