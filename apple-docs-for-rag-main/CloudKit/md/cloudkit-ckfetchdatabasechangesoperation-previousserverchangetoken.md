

- CloudKit
- CKFetchDatabaseChangesOperation
-  previousServerChangeToken 

Instance Property

# previousServerChangeToken

The server change token.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
@NSCopying
var previousServerChangeToken: CKServerChangeToken? { get set }
```

## Discussion

Assign the token you receive from the fetchDatabaseChangesCompletionBlock to this property. Doing so yields only the changes that occur after your most recent fetch operation. If you specify `nil` for this parameter, the operation fetches all changes.

## See Also

### Configuring the Operation

var fetchAllChanges: Bool

A Boolean value that indicates whether to send repeated requests to the server.

var resultsLimit: Int

The maximum number of results that the operation fetches.

