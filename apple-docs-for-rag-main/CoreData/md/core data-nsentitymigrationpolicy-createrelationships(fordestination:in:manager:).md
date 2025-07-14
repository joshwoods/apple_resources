

- Core Data
- NSEntityMigrationPolicy
-  createRelationships(forDestination:in:manager:) 

Instance Method

# createRelationships(forDestination:in:manager:)

Constructs the relationships between the newly-created destination instances.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func createRelationships(
    forDestination dInstance: NSManagedObject,
    in mapping: NSEntityMapping,
    manager: NSMigrationManager
) throws
```

## Parameters 

`dInstance`  

The destination instance for which to create relationships.

`mapping`  

The mapping object in use.

`manager`  

The migration manager performing the migration.

## Discussion

You can use this stage to (re)create relationships between migrated objects—you use the association lookup methods on the NSMigrationManager instance to determine the appropriate relationship targets.

## See Also

### Customizing Stages of the Mapping Life Cycle

func begin(NSEntityMapping, with: NSMigrationManager) throws

Sets up state information before the start of a given entity mapping.

func createDestinationInstances(forSource: NSManagedObject, in: NSEntityMapping, manager: NSMigrationManager) throws

Creates the destination instance(s) for a given source instance.

func endInstanceCreation(forMapping: NSEntityMapping, manager: NSMigrationManager) throws

Indicates the end of the instance creation stage for the specified entity mapping, and the precursor to the next migration stage.

func endRelationshipCreation(forMapping: NSEntityMapping, manager: NSMigrationManager) throws

Indicates the end of the relationship creation stage for the specified entity mapping.

func performCustomValidation(forMapping: NSEntityMapping, manager: NSMigrationManager) throws

Provides the option to perform custom validation on migrated objects during the validation stage of the entity migration policy.

func end(NSEntityMapping, manager: NSMigrationManager) throws

Performs cleanup at the end of the migration, from any phase of the mapping.

