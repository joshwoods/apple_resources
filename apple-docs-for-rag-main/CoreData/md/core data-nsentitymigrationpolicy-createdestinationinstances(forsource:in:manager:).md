

- Core Data
- NSEntityMigrationPolicy
-  createDestinationInstances(forSource:in:manager:) 

Instance Method

# createDestinationInstances(forSource:in:manager:)

Creates the destination instance(s) for a given source instance.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func createDestinationInstances(
    forSource sInstance: NSManagedObject,
    in mapping: NSEntityMapping,
    manager: NSMigrationManager
) throws
```

## Parameters 

`sInstance`  

The source instance for which to create destination instances.

`mapping`  

The mapping object in use.

`manager`  

The migration manager performing the migration.

## Discussion

This method is invoked by the migration manager on each source instance (as specified by the sourceExpression in the mapping) to create the corresponding destination instance(s). It also associates the source and destination instances by calling `NSMigrationManager`’s associate(sourceInstance:withDestinationInstance:for:) method.

### Special Considerations

If you override this method and do not invoke `super`, you must invoke `NSMigrationManager`’s associate(sourceInstance:withDestinationInstance:for:) to associate the source and destination instances as required. .

## See Also

### Customizing Stages of the Mapping Life Cycle

func begin(NSEntityMapping, with: NSMigrationManager) throws

Sets up state information before the start of a given entity mapping.

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

