

- Core Data
- NSMigrationManager
-  currentEntityMapping 

Instance Property

# currentEntityMapping

The entity mapping currently being processed.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var currentEntityMapping: NSEntityMapping { get }
```

## Discussion

Each entity is processed a total of three times—instance creation, relationship creation, and validation.

### Special Considerations

You can observe this value using key-value observing.

## See Also

### Monitoring a Migration’s Progress

var migrationProgress: Float

A number between `0` and `1` that indicates the proportion of completeness of the migration.

