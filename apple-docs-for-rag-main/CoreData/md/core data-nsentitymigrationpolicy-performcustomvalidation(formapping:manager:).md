

- Core Data
- NSEntityMigrationPolicy
-  performCustomValidation(forMapping:manager:) 

Instance Method

# performCustomValidation(forMapping:manager:)

Provides the option to perform custom validation on migrated objects during the validation stage of the entity migration policy.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func performCustomValidation(
    forMapping mapping: NSEntityMapping,
    manager: NSMigrationManager
) throws
```

## Parameters 

`mapping`  

The mapping object in use.

`manager`  

The migration manager performing the migration.

## Discussion

This method is called before the default save validation is performed by the framework.

If you implement this method, you must manually obtain the collection of objects you are interested in validating.

## See Also

### Customizing Stages of the Mapping Life Cycle

func begin(NSEntityMapping, with: NSMigrationManager) throws

Sets up state information before the start of a given entity mapping.

func createDestinationInstances(forSource: NSManagedObject, in: NSEntityMapping, manager: NSMigrationManager) throws

Creates the destination instance(s) for a given source instance.

func endInstanceCreation(forMapping: NSEntityMapping, manager: NSMigrationManager) throws

Indicates the end of the instance creation stage for the specified entity mapping, and the precursor to the next migration stage.

func createRelationships(forDestination: NSManagedObject, in: NSEntityMapping, manager: NSMigrationManager) throws

Constructs the relationships between the newly-created destination instances.

func endRelationshipCreation(forMapping: NSEntityMapping, manager: NSMigrationManager) throws

Indicates the end of the relationship creation stage for the specified entity mapping.

func end(NSEntityMapping, manager: NSMigrationManager) throws

Performs cleanup at the end of the migration, from any phase of the mapping.

