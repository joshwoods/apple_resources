

- Core Data
- NSMigrationManager
-  cancelMigrationWithError(\_:) 

Instance Method

# cancelMigrationWithError(\_:)

Cancels the migration with a given error.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func cancelMigrationWithError(_ error: any Error)
```

## Parameters 

`error`  

An error object that describes the reason why the migration is canceled.

## Discussion

You can invoke this method from anywhere in the migration process to abort the migration. Calling this method causes migrateStore(from:sourceType:options:with:toDestinationURL:destinationType:destinationOptions:) to abort the migration and return `error`—you should provide an appropriate error to indicate the reason for the cancellation.

## See Also

### Aborting a Migration

func reset()

Resets the association tables for the migration.

