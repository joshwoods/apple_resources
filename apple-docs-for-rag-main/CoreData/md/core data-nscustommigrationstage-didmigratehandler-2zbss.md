

- Core Data
- NSCustomMigrationStage
-  didMigrateHandler 

Instance Property

# didMigrateHandler

The handler to execute after the stage runs.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+Swift 5.8+

``` source
var didMigrateHandler: ((NSStagedMigrationManager, NSCustomMigrationStage) throws -> Void)? { get set }
```

## Discussion

Use this handler to perform any cleanup tasks on the persistent store’s data after the migration has run. Access the store using the container property of the handler’s `migrationManager` parameter.

## See Also

### Assigning event handlers

var willMigrateHandler: ((NSStagedMigrationManager, NSCustomMigrationStage) throws -> Void)?

The handler to execute before the stage runs.

