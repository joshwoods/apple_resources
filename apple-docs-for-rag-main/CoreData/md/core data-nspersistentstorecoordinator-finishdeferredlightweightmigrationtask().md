

- Core Data
- NSPersistentStoreCoordinator
-  finishDeferredLightweightMigrationTask() 

Instance Method

# finishDeferredLightweightMigrationTask()

Executes a single pending task of a deferred lightweight migration.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
func finishDeferredLightweightMigrationTask() throws
```

## Discussion

Note

Enable deferred lightweight migrations before using this method. For more information, see NSPersistentStoreDeferredLightweightMigrationOptionKey.

## See Also

### Deferring a store’s migrations

let NSPersistentStoreDeferredLightweightMigrationOptionKey: String

The key for enabling deferred lightweight migrations.

func finishDeferredLightweightMigration() throws

Executes all remaining tasks of a deferred lightweight migration.

