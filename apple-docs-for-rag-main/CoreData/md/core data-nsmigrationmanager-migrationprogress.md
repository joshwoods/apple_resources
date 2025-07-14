

- Core Data
- NSMigrationManager
-  migrationProgress 

Instance Property

# migrationProgress

A number between `0` and `1` that indicates the proportion of completeness of the migration.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var migrationProgress: Float { get }
```

## Discussion

If a migration is not taking place, this property is `1`. You can observe this value using key-value observing.

## See Also

### Monitoring a Migration’s Progress

var currentEntityMapping: NSEntityMapping

The entity mapping currently being processed.

