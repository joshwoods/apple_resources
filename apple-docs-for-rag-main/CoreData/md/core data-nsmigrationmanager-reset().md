

- Core Data
- NSMigrationManager
-  reset() 

Instance Method

# reset()

Resets the association tables for the migration.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func reset()
```

## Discussion

This method does not reset the source or destination contexts.

## See Also

### Aborting a Migration

func cancelMigrationWithError(any Error)

Cancels the migration with a given error.

