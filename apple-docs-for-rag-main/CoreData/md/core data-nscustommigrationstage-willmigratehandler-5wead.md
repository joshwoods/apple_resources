

- Core Data
- NSCustomMigrationStage
-  willMigrateHandler 

Instance Property

# willMigrateHandler

The handler to execute before the stage runs.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+Swift 5.8+

``` source
var willMigrateHandler: ((NSStagedMigrationManager, NSCustomMigrationStage) throws -> Void)? { get set }
```

## Discussion

Use this handler to prepare the persistent store’s data for the pending migration. Access the store using the container property of the handler’s `migrationManager` parameter.

## See Also

### Assigning event handlers

var didMigrateHandler: ((NSStagedMigrationManager, NSCustomMigrationStage) throws -> Void)?

The handler to execute after the stage runs.

