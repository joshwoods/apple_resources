

- CloudKit
- CKFetchDatabaseChangesOperation
-  init(previousServerChangeToken:) 

Initializer

# init(previousServerChangeToken:)

Creates an operation for fetching database changes.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
convenience init(previousServerChangeToken: CKServerChangeToken?)
```

## Parameters 

`previousServerChangeToken`  

The change token that CloudKit uses to determine which database changes to return.

## Discussion

After creating the operation, assign a handler to the fetchDatabaseChangesCompletionBlock property so that you can process the operation’s results.

If this is your first fetch, or if you want to refetch all zones, pass `nil` for the change token. If you provide a change token from a previous CKFetchDatabaseChangesOperation, CloudKit returns only the zones with changes since that token. The per-database CKServerChangeToken isn’t the same as the per-record zone CKServerChangeToken from CKFetchRecordZoneChangesOperation.

## See Also

### Creating an Operation

init()

Creates an empty fetch database changes operation.

